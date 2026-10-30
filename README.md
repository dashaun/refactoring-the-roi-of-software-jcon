# Refactoring the ROI of Software

**Lessons from the Frontlines of OpenRewrite Adoption**  
DaShaun Carter · JCON USA 2026 · Atlanta · October 26–29, 2026

A presentation about making modernization a continuous workflow, using OpenRewrite recipes to share migration decisions, and keeping software on the latest patch (N-0).

The slides cover:

- Refactoring as part of CI/CD, with a dedicated remediation workflow.
- AI-assisted recipe creation and reusable, versioned transformations.
- Good, Better, Best approaches to modernization across repositories.
- A Spring Boot 2.7 / Java 8 upgrade to Spring Boot 4.x / Java 25, comparing Spring Application Advisor, Codex, and Claude.
- Behavioral verification and the cost of reviewing migration decisions.

## View the slides

Open [docs/index.html](docs/index.html) in a browser. The presentation includes its scripts, styles, images, and captured result tables. No build, API keys, or network connection is required.

Use the arrow keys or Space to navigate, Esc for the overview, and F for fullscreen. To print or save a PDF, open `docs/index.html?print-pdf` in Chrome or Edge and use the browser's print dialog with landscape orientation and background graphics enabled.

To serve locally with a JDK that includes `jwebserver`:

```sh
jwebserver -b 127.0.0.1 -p 8123 -d docs
```

Then open <http://localhost:8123/>.

## Publish

The `docs/` directory is the complete static site. Upload its contents to any static host, or configure GitHub Pages to deploy from the `main` branch and `/docs` folder. No build step is needed.

## Reading the results

The captured tables describe a small Java upgrade experiment, not a controlled vendor speed ranking. Models, workflow settings, and release channels differ. Repeated runs compare tracked patches from two runs per tool; they do not establish a consistency rate. Token accounting differs by CLI, and zero tokens does not mean zero total cost.

The review-cost example assumes 400 pull requests at 30 minutes each. It is illustrative, not measured savings. Every recipe-generated change still requires testing and review.

Advisor is Spring Application Advisor, a Broadcom product built on OpenRewrite. DaShaun works at Broadcom.

## Credits

Presentation runtime: [reveal.js](https://revealjs.com), distributed under the MIT license. See [third-party notices](THIRD_PARTY_NOTICES.md).

[dashaun.com](https://dashaun.com) · [OpenRewrite](https://github.com/openrewrite)
