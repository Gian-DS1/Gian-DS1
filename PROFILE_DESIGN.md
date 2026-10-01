# Profile visuals

The city-pop terminal design, particle banner generator and radar renderer are
adapted from [macu-dev/macu-dev](https://github.com/macu-dev/macu-dev), reference
commit `2eaa44d`. Giancarlos's previous README supplies the profile facts, project
descriptions, toolbox and background. The portrait is his GitHub avatar captured
on 2026-10-01; no other person's portrait or contact details are included.

## Regenerate the banner

From the repository root, with Python 3.10 or later:

```sh
python -m pip install -r scripts/banner/requirements.txt
python scripts/banner/generate.py
```

Edit `YAML_ROWS` in `scripts/banner/generate.py` to update the profile panel.
Replace `assets/source/portrait.png` to change the portrait. Local Python
monogram and SQL database silhouettes are in `scripts/banner/logos/`.
The generator writes both light and dark animated SVGs; the README selects them
using `<picture>` and `prefers-color-scheme`. Generated SVGs are committed so the
profile does not need a live image-generation server or an API secret.

## Regenerate the radars

The radar renderer uses only Python's standard library:

```sh
python scripts/radar.py --data assets/skills.json -o assets/radar --values --size 290
python scripts/radar.py --data assets/langmix.json -o assets/radar-langs --size 290
```

`assets/skills.json` records category coverage across the four featured projects,
not skill ratings. A category value is its project count divided by four times
100: pipelines (Stock Screener, Zomato), machine learning (Stock Screener), web
apps (Stock Screener, FinTrack, LIENZO), finance (Stock Screener, FinTrack),
orchestration (Zomato), agent tooling (LIENZO). Update the data and the README's
caption and alternative text together when featured projects change.

`assets/langmix.json` is a snapshot of GitHub language byte counts across public,
non-fork, non-archived repositories. Axes use `100 * sqrt(bytes / largest_bytes)`;
they represent relative code volume, not percentages or proficiency. HTML, CSS,
Shell, Makefile, Dockerfile and Batchfile are excluded. To render a fresh live
snapshot directly (update the README date and alternative text as needed):

```sh
python scripts/radar.py --github Gian-DS1 --limit 6 --size 290 --title "Gian-DS1 · public language mix" -o assets/radar-langs
```

Keep `assets/langmix.json` in sync if using JSON to regenerate later. An optional
`GH_TOKEN` or `GITHUB_TOKEN` environment variable raises GitHub API rate limits;
never commit its value.

## Existing statistics

`.github/workflows/stats-cards.yml` continues to refresh the original local
statistics cards daily. This customization does not change that workflow.
Typing text, technology icons and badges use the same external
image services as the reference profile; the main banner, terminal and radars
are local SVGs. Profile facts and project descriptions remain readable as text.
