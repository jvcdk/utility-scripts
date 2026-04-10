# Utility scripts

A small collection of developer utility scripts for Linux desktop environments.

## Tools

### webappify

Converts any website into a standalone desktop application with an isolated browser profile.

- Creates `.desktop` entries and browser profiles in `~/.webapp/`
- Fetches icons automatically from HTML metadata (manifest, Open Graph, favicons)
- Supports Chrome, Chromium, Brave, Edge, and Vivaldi

```sh
webappify add https://example.com
webappify list
webappify remove example
```

**Dependencies:** Python 3, one of ImageMagick or `rsvg-convert` (for icon conversion), a supported Chromium-based browser.

---

### git-fixup

Streamlines the fixup commit workflow. Detects which recent commit last touched your staged files and creates a `fixup!` commit, then optionally rebases.

```sh
git fixup          # auto-detect target commit from staged files
git fixup <ref>    # fix up a specific commit
```

**Dependencies:** Bash, Git.

---

### git-blame-pending

Reports which commits last touched the lines you have modified but not yet staged (single-line edits only).

```sh
git blame-pending
```

**Dependencies:** Python 3, Git.

## License

MIT
