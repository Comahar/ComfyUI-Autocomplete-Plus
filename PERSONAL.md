# Personal patch branch

Runs on top of upstream `main` with unmerged fixes cherry-picked for day-to-day ComfyUI use.

| Change | Upstream | Files |
|--------|----------|-------|
| App mode / Nodes 2.0 attachment | PR [#85](https://github.com/newtextdoc1111/ComfyUI-Autocomplete-Plus/pull/85) (Comahar) | `web/js/main.js` |
| Dark theme on Vue frontend | PR [#82](https://github.com/newtextdoc1111/ComfyUI-Autocomplete-Plus/pull/82) | `web/css/autocomplete-plus.css` |
| Popup position when textarea scrolled | PR [#74](https://github.com/newtextdoc1111/ComfyUI-Autocomplete-Plus/pull/74) | `web/js/autocomplete.js` |
| Subpath / reverse-proxy URLs | PR [#78](https://github.com/newtextdoc1111/ComfyUI-Autocomplete-Plus/pull/78) | `web/js/main.js`, `web/js/utils.js` |

## Update from upstream

```bash
git fetch upstream
git checkout personal
git merge upstream/main   # resolve if needed, re-cherry-pick if cleaner
git push origin personal
```

## Install

```bash
git clone -b personal https://github.com/Comahar/ComfyUI-Autocomplete-Plus.git \
  custom_nodes/ComfyUI-Autocomplete-Plus
```
