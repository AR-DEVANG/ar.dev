---
ai-generated: true
date: 2026-09-13
---
# Implementation contract

## Structure

`site/index.html` is the only application entry point. Inline CSS and JavaScript; local responsive WebP assets. No build system or runtime API. Serve only `site/`; development documents and raw sources sit beside it.

One scrolling page: introduction, Work, Reimagined, Updates, About. Projects use native `details` so their technical context remains accessible without scripting. Three projects: TONY, Journey in Motion, and the Way Side Amenities academic archive. Do not conflate the last with SHK internship work or label it as a UHPC thesis.

## Behavior

- Native anchors and a sticky navigation bar. Current section is marked progressively with IntersectionObserver; navigation itself needs no JavaScript.
- Comparison: native range input, 0–100 original visibility, initial 42%; arrow keys change by one. Two pressed-state study buttons update the generated image and live caption while preserving range position. A separate native disclosure offers all three full images, including without JS.
- Updates: semantic HTML entries newest first. Filter by `all`, `ardev`, `tony`, `fellowship`, `wayside`. Initially show three matching entries; reveal three more at a time. Filtering resets pagination. Announce counts in a status region; hide the reveal control when exhausted and transfer focus to the first newly revealed entry. Without JS show every note.
- Appearance: System / Light / Dark select. Reduced-motion checkbox only adds reduction; it never disables system reduction. Save preferences in localStorage, tolerate inaccessible storage, and work for the current tab regardless.
- Contact: existing professional mailto address. Research video opens as a user-initiated external YouTube link; no embed or background request.

## Media and truth

All exported images stay below 1 MB; width variants are 800 and up to 1600 px without upscaling. Strip metadata on export. Use image source dimensions in srcset descriptors. Reference documents and generation prompts stay private. Source originals are copied, not modified.

No corresponding verified architectural walkthrough was found in the inspected thesis-render and final-submission folders. The unrelated Futala video is not used for the thesis. The image comparison provides the immersive section, and the fellowship film remains externally linked. No video playback state is fabricated.

## Validation and handoff

Check the full navigation, all details, every filter, reveal-all/reset behavior, both studies, comparison endpoints and keyboard controls, appearance persistence, reduced motion, mobile overflow, local asset loading and console output. Run `python3 qa/check.py`; add `--http` against the local preview server for HTTP checks. Browser results are recorded in `qa/RESULTS.md`.

Deployment and domain registration are excluded. The previous studies are preserved. The new project is the current implementation; older contracts describe their historical studies.
