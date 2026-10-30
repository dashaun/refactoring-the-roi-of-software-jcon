# Repository guidance

This repository distributes the public static presentation "Refactoring the ROI of Software: Lessons from the Frontlines of OpenRewrite Adoption" from JCON USA 2026.

The presentation covers continuous modernization in CI/CD, OpenRewrite recipes, AI-assisted migrations, N-0 patching, adoption practices, and captured Spring Boot / Java upgrade results. Keep `README.md` aligned with the slides.

- `docs/index.html` contains the slides and presentation styles.
- `docs/images/` contains presentation artwork.
- `docs/reveal.js/` contains the bundled presentation runtime.
- Keep the site static, self-contained, and usable without network access.
- Keep preparation notes, speaker notes, TODO lists, execution logs, credentials, and live-demo infrastructure out of this distribution.
- Preserve third-party license notices.
- Keep the captured results, methodology caveats, and product affiliation disclosure together when editing the comparison slides.
- Verify local asset references after changes; external reading links must not be required to render the slides.
- Prefer Java for any necessary automation; shell is fine for thin launchers.
- Do not push or publish without the user's approval.
