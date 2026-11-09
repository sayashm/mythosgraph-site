# MythosGraph portfolio

This repository publishes the static portfolio at https://sayashm.github.io/mythosgraph-site/.
It contains only built website assets, recorded pilot data embedded in those assets,
and a GitHub Pages deployment workflow. The application source, credentials, raw
documents, vector index, and Docker package remain in the private MythosGraph repository.

To update the site from the private source repository, run `npm ci` and `npm run build`
in `web/`, then run `python3 scripts/export_public_site.py --output PATH` from the
source root, replacing `PATH` with a clean directory. Copy that directory's contents
into this repository, commit, and push `main`. The workflow deploys `site/`.
