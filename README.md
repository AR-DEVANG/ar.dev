# ar.dev

Source for **[devangchawhan.com](https://devangchawhan.com)**, the portfolio of Devang Chawhan: architecture, materials research, intelligent tools, and the interfaces between people and places.

One hand-written HTML page. No framework, no build step, no dependencies, no runtime API.

## Preview

Run from this directory:

```sh
python3 -m http.server 8765 --bind 127.0.0.1 --directory site
```

Open http://127.0.0.1:8765. Serve **only `site/`**. The page also works as a local HTML file and under a repository subpath.

## Layout

| Path | Holds |
| --- | --- |
| `site/` | The published page, favicon, and image assets |
| `Design_System/` | The design contracts: philosophy, content record, tokens, build brief |

## Editing

Source facts and dated notes are recorded in `Design_System/CONTENT.md`; update that record when changing public copy. The update entries are semantic HTML in `site/index.html`, sorted newest first. Add entries with a real date and an existing `data-project` value (`ardev`, `tony`, `fellowship`, `wayside`). The browser filters them and reveals three at a time. All entries remain accessible without JavaScript.

Source material, generation prompts, and local checks are kept out of this repository.

## Deployment

Every push to `main` deploys `site/` to https://devangchawhan.com through Vercel. There is no build.

## Boundaries

TONY is a prototype, the architecture is academic design, and generated studies are labeled as such. Only the owned contact address and the fellowship reflection link are exposed. The selected architecture has no verified walkthrough footage, so this release uses still-image comparison rather than unrelated archival video. Nothing autoplays.
