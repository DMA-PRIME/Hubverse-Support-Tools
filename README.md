# Hubverse Support Toolkit

The Hubverse Support Toolkit is a collection of browser-based utilities from DMA-PRIME at Clemson University. The tools are intended to help modeling teams complete technical pieces of Hubverse submissions without requiring programming.

The toolkit is currently in beta testing. Generated files should always be checked against the selected hub's current instructions and official validation process before submission. Feedback and possible errors can be sent to [ambleic@clemson.edu](mailto:ambleic@clemson.edu?subject=Hubverse%20Support%20Toolkit%20feedback).

## Publish with GitHub Pages

This repository is deliberately organized so GitHub Pages publishes only the website files in `docs/`.

1. Upload this repository structure to GitHub.
2. Open **Settings → Pages** in the repository.
3. Under **Build and deployment**, select **Deploy from a branch**.
4. Select the `main` branch and the `/docs` folder.
5. Save the settings. GitHub will display the website address when deployment finishes.

Do not select the repository root as the publishing source. Selecting `/docs` keeps sibling project folders off the GitHub Pages website.

## Repository structure

```text
Hubverse-Support-Toolkit/
├── README.md
├── LICENSE
├── docs/                         # Published website
│   ├── index.html                # Toolkit homepage
│   ├── .nojekyll
│   ├── tools/
│   │   └── metadata-generator/
│   │       └── index.html        # Online tool
│   └── offline/
│       ├── README.txt
│       └── Hubverse-Metadata-Generator.html
└── project/                      # Not published by GitHub Pages
```

Files outside `docs/` are not served on the Pages website. However, they are still visible in GitHub when the repository is public. Confidential, restricted, or private project material should be stored in a separate private repository.

## Use a tool offline

Standalone tool files are available in `docs/offline/` and from the download buttons on the toolkit homepage.

1. Download the desired `.html` file.
2. Save it locally.
3. Double-click it to open it in a modern browser.

No installation or local web server is required. The Model Metadata Generator's application code, styles, tutorial, and hub schema snapshots are contained inside its HTML file. Links to external documentation still require an internet connection.

## Add another tool

For each future standalone tool:

1. Create `docs/tools/tool-name/index.html` for the online version.
2. Place a self-contained copy in `docs/offline/Descriptive-Tool-Name.html`.
3. Add a new tool card to `docs/index.html` with both an **Open tool** link and a **Download standalone HTML** link.
4. Test the online page from the repository's GitHub Pages URL and test the offline copy by opening it directly from a computer.

Keep paths on the homepage relative so the site works at `https://USERNAME.github.io/REPOSITORY/`.

## Official resources

- [Hubverse](https://hubverse.io/)
- [Hubverse documentation](https://docs.hubverse.io/)
- [DMA-PRIME](https://dma-prime.org/)
- [Clemson University](https://www.clemson.edu/)
