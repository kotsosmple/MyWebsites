# Project Guidelines

## Structure
- This is a root-level static website. `index.html` is the home page; the other HTML files are standalone pages for villas, booking, contact, the magazine, and error/coming-soon states.
- Pages generally keep their CSS and JavaScript inline. Follow the nearest page's existing structure and styling when making a focused change; avoid introducing shared tooling or restructuring pages unless requested.
- Local images, audio, and video are stored at the repository root. Preserve relative paths and verify referenced filenames, including spaces, against the actual files.

## Workflow
- There is no repository-defined build, test, or preview command. Do not invent one; validate changed pages in a browser at desktop and mobile widths when practical.
- `netlify.toml` configures response headers and caching, but does not define a build or publish directory. Keep deployment assumptions explicit.
- Check the target page and its nearest equivalent before editing; villa pages share recurring patterns but also contain page-specific markup and behavior.

## Behavior To Verify
- Do not describe the contact form as submitting data: its current handler displays an alert and prevents submission.
- Do not describe booking as a completed transaction: the current booking handler is a demonstration flow.
- Verify `LINK_PLAYLIST` placeholders and links that point outside this repository before changing or relying on them; their intended destinations are not established here.
