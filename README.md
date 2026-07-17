# NovSucks

A community-maintained knowledge base for **Novritsch** airsoft replicas — Bills of Materials, 3D-printable spare/upgrade parts, and links to the (often identical) source products sold on AliExpress and elsewhere.

Novritsch replicas are frequently rebrands of existing OEM designs manufactured by other factories. When you know the underlying OEM/factory version, you can often source spare parts, upgrades, or the whole replica itself for a fraction of the price. This repo collects that knowledge in one place so the community doesn't have to keep rediscovering it.

## ⚠️ Disclaimer

- This is a hobbyist project about **airsoft**, a legal sport/hobby in most jurisdictions (always check your local laws on replica ownership/import, as these do vary by country). Nothing here concerns illegal activity.
- This project is **not affiliated with, endorsed by, or connected to Novritsch** in any way. "Novritsch" and related product names are used solely to identify the products being referenced (nominative fair use).
- All content here is **community-submitted, unofficial, and provided for educational/informational purposes**. Accuracy is not guaranteed — always verify compatibility before buying or printing anything.
- Linked third-party listings (AliExpress, etc.) are **not vetted or endorsed**. Sellers, prices, and product accuracy change constantly — do your own due diligence.
- No claim is made that Novritsch's business practices are unlawful or improper. The premise here is simply that many of their products appear to share origins with parts/products available more cheaply elsewhere, which is common practice across the airsoft industry (and consumer goods generally).
- This repo contains no copyrighted files belonging to Novritsch (manuals, marketing images, proprietary CAD, etc.) — only community-authored documentation, original/derivative 3D models, and links.

If you are a rights holder and have a concern about specific content, please open an issue and it will be addressed.

## What's in here

| Content | Where |
|---|---|
| Bill of Materials per replica | `<product>/bom.md` |
| 3D-printable files (STL + editable source) | `<product>/3d-print-files/` |
| AliExpress / alternative source links | `<product>/links.md` |
| General guides (not tied to one product) | `guides/` |

## Repo structure

```
NovSucks/
├── ssx303/                  # one folder per Novritsch product
│   ├── README.md            # overview, notes, known quirks
│   ├── bom.md                # Bill of Materials (Markdown table)
│   ├── links.md              # AliExpress / OEM alternative links
│   └── 3d-print-files/
│       ├── stl/               # print-ready meshes
│       └── source/            # editable CAD source (STEP/F3D/SCAD/...)
├── ssx23/
├── ssg24/
├── ssp18/
├── ssp1/
├── ssu12/
├── antifog-unit/             # AntiFog Unit Gen2 (BB Proof), model E164B2
├── compact-chrono/           # Compact Chrono, model E308
├── _template/                # copy this folder to add a new product
├── guides/                  # cross-cutting how-tos (not product specific)
└── CONTRIBUTING.md
```

Product folders are named after the Novritsch model designation in lowercase kebab-case (e.g. `ssx303`, `ssg24`).

This list of products is a starting point, not the full lineup — see [Contributing](CONTRIBUTING.md) for how to add a missing product.

## Contributing

PRs adding/correcting BOMs, links, or 3D files are welcome. See [CONTRIBUTING.md](CONTRIBUTING.md) for folder conventions and format expectations before submitting.

## License

This repository is licensed under the [CC BY-NC-SA 4.0 International Public License](LICENSE). By contributing, you agree to license your contribution under the same terms.
