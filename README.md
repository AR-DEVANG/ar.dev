# ar.dev

An independent implementation of the 13 September 2026 approved design direction. Earlier studies are preserved in `../ar-dev-replit/` and the Ideaverse project.

## Preview

Run from this directory:

```sh
python3 -m http.server 8765 --bind 127.0.0.1 --directory site
```

Open http://127.0.0.1:8765. Serve **only `site/`**. No build, dependencies, account, backend, or runtime API is required. The page also works as a local HTML file and under a repository subpath.

## Editing

The design contracts live in `Design_System/`. Source facts and dated notes are recorded in `CONTENT.md`; update that record when changing public copy. The five update entries are semantic HTML in `site/index.html`, sorted newest first. Add entries with a real date and an existing `data-project` value (`ardev`, `tony`, `fellowship`, `wayside`). The browser filters them and reveals three at a time. All entries remain accessible without JavaScript.

`private/` holds copied sources, generation prompts, original-to-export provenance, and factual evidence paths. It must stay outside the served/deployed directory. `qa/` holds local checks. Both are ignored by Git.

## Boundaries

Local preview only; no deployment or domain registration. TONY is a prototype, architecture is academic design, and generated studies are labeled. Only the already-used professional email and existing fellowship reflection link are exposed. There are no invented GitHub or social links.

The selected architecture has no matched, verified walkthrough in the inspected source folders. This release uses still-image comparison and an external link to the fellowship reflection rather than attaching unrelated archival footage. Nothing autoplays.
