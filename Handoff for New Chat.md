# Voice Command Atlas Pages Handoff

Updated: 2026-07-16

## New Chat Rule

Read this file before changing the public Voice Command Atlas support, privacy, or release-summary pages.

## Project State

- Local path: `/Users/briscoe/Documents/MacApps/Voice-Command-Atlas-Pages`
- GitHub repo: `https://github.com/wch1zpnk/Voice-Command-Atlas-Pages`
- Branch: `main`
- Hosting: GitHub Pages from the repository root
- Public root: `https://wch1zpnk.github.io/Voice-Command-Atlas-Pages/`
- App Store Connect privacy URL: `https://wch1zpnk.github.io/Voice-Command-Atlas-Pages/privacy.html`
- Latest published functional commit: `1e44446 Correct App Store export workflow pages`

## Current Public Behavior

- `privacy.html` says the Mac App Store version reads only the `.voicecontrolcommands` export explicitly chosen in a standard macOS Open dialog.
- Edits affect only the selected export until it is re-imported through Voice Control's Options menu.
- `support.html` documents Export Custom Commands, Import Custom Commands, and reopening the main window with Window > Show Voice Command Atlas Window or Command-1.
- `index.html` identifies the current corrected release/build line as `1.0.1` and describes the selected-export workflow.
- Do not restore the old direct `~/Library/Preferences/...CustomCommands.plist` wording or claims that the Mac App Store app restarts Voice Control helper processes.

## Verification Completed

- Local `git diff --check` and the three-page local link/asset scan passed.
- Local stale-workflow and private-string scans passed.
- GitHub Pages run `29543748214` completed successfully for commit `1e44446`. GitHub reported only its existing non-blocking Node.js 20 deprecation annotation.
- Cache-busted public readback returned HTTP `200` for `index.html`, `privacy.html`, and `support.html` and confirmed the corrected export/import and Command-1 wording.
- Live in-app-browser verification confirmed the privacy page has no horizontal overflow, no console warnings/errors, no stale preference path, and visible selected-export/re-import wording.

## Submission Boundary

- Publishing these pages does not submit the app for review.
- The corrected build `1.0.1` is already attached to App Store Connect version `1.0`.
- The user reserved the App Store Connect `Update Review` action for their own final inspection and click.
