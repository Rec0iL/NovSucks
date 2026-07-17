# Contributing

Thanks for helping build this out. This repo is only useful if the data in it is accurate, so please double-check anything you submit (measurements, part fit, links) before opening a PR.

## Adding a new product

1. Copy the `_template/` folder and rename it to the product's model designation in lowercase kebab-case (e.g. `ssx303`, `antifog-unit`).
2. Fill in `README.md`, `bom.md`, and `links.md` inside it using the formats below.
3. Drop any 3D files into `3d-print-files/stl/` (print-ready) and, if available, `3d-print-files/source/` (editable CAD: STEP, F3D, SCAD, etc.).
4. Add the new folder to the structure list in the root [README.md](README.md).

## Folder layout per product

```
<product>/
├── README.md       # short overview: what it is, known quirks, links to more info
├── bom.md          # Bill of Materials
├── links.md        # AliExpress / OEM alternative sources
└── 3d-print-files/
    ├── stl/          # print-ready meshes
    └── source/       # editable CAD source, if you have it
```

## BOM format (`bom.md`)

Use a Markdown table. One row per part. Keep the columns below; add extra columns if useful (e.g. "Notes").

```markdown
| Part | Novritsch part # | OEM/AliExpress equivalent | Notes |
|---|---|---|---|
| Nozzle | N/A | [Seller listing](https://...) | Fits without modification |
```

Only include information you've verified yourself or can cite a source for. If you're unsure a part is actually equivalent, say so in the Notes column rather than presenting it as confirmed.

## Link list format (`links.md`)

```markdown
# <Product> — Alternative Sources

- [Seller/listing name](https://...) — what it is, price seen, any caveats
  - Search term if the link dies: **"..."**
```

Prefer direct product listing links over shop homepages. Note the date you found the link if prices/availability are likely to change.

AliExpress links rot fast (listings get delisted or reshuffled). Always add a fallback search term alongside the link — the product's actual title/model name (e.g. an OEM model number), or a generic phrase that reliably surfaces equivalent listings — so people can still find the item once the link is dead.

## 3D print files

- Only submit files you made yourself, have permission to share, or that are already open-licensed (say which license in the file's folder or a short note in `README.md`).
- Do not upload Novritsch's own proprietary files or reverse-engineered exact copies of their trademarked design elements — this repo is for original/derivative parts (adapters, fixes, upgrades), not piracy of their CAD.
- Mention the slicer settings you used (layer height, infill, material) in the product `README.md` if they matter for fit/strength.

## General guides

Content that isn't tied to one specific product (tools, how to identify a source factory, general printing tips, etc.) goes in [guides/](guides/) instead of a product folder.

## Pull requests

- Keep PRs scoped to one product or one guide where possible — easier to review.
- Explain in the PR description how you verified the info (own purchase, measured original part, seller confirmation, etc.).
- Broken or dead links, incorrect BOMs, and outdated info are welcome as issues too, even without a fix in hand.
