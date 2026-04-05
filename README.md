# Emerald Legacy Workshop

Welcome to the **Emerald Legacy Workshop**! This repository serves as the central registry for community-driven content used by the Emerald Legacy Launcher.

## About
The Workshop is a free, open-source alternative to the Minecraft Marketplace. It allows the community to share:
- **Skins Packs**: High-quality character skins.
- **Texture Packs**: Resource updates for Title Updates.
- **DLCs**: Expansion packs, maps, etc.

## How to Contribute

We welcome contributors! To add your content to the workshop:

1. **Fork this repository.**
2. **Upload your content**: Create a subfolder and place your assets (zips, thumbnails) in the `assets/` folder or host them via GitHub Releases in your own repo.
3. **Update `workshop.json`**: Add your item to the list following the schema below.
4. **Submit a Pull Request**: Our team will review your submission for quality and safety.

## Schema Details

Every item in `workshop.json` must follow this structure:

| Field | Type | Description |
|---|---|---|
| `id` | String | A unique identifier (kebab-case). |
| `name` | String | Display name of the item. |
| `author` | String | Your name or organization. |
| `description`| String | A short summary of what the item does. |
| `category` | String | Must be `Skins`, `Packs`, or `DLC`. |
| `thumbnail` | URL | A 1:1 image (PNG/JPG) for the preview. |
| `downloadUrl`| URL | Direct link to a `.zip` file of the content, it can be directly inside your folder on /assets/ or a repo's release. |
| `version` | String | Semantic versioning (e.g. `1.0.0`). |

## License
By contributing to this repository, you agree to license your manifest entries under the **MIT License**. The content itself (skins/packs) must be compatible with FOSS distribution.
