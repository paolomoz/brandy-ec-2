# EDS Block Collection Demo

This project demonstrates all blocks from the Adobe Experience Manager Edge Delivery Services block collection.

## Environments
- Preview: https://main--{repo}--{owner}.aem.page/
- Live: https://main--{repo}--{owner}.aem.live/

## Available Blocks

This project includes the following blocks:
- **Hero** - Full-width hero sections with images and CTAs
- **Cards** - Card grid layouts for features and content
- **Columns** - Multi-column responsive layouts
- **Accordion** - Expandable/collapsible FAQ sections
- **Tabs** - Tabbed content interfaces
- **Table** - Data tables with variants (striped, bordered)
- **Video** - YouTube/Vimeo video embeds with placeholders
- **Carousel** - Image/content sliders with navigation
- **Embed** - Generic embed for external content
- **Search** - Site search functionality
- **Footer** - Site footer
- **Header** - Site header
- **Fragment** - Reusable content fragments

## Documentation

### Project-Specific Documentation

**IMPORTANT**: When creating content pages for this project:
1. See [Block Structure Guide](docs/BLOCK-STRUCTURE.md) for complete markdown formatting rules
2. Reference [blocks-demo.md](blocks-demo.md) for working examples of all blocks
3. Review [.eds-project.md](.eds-project.md) for quick reference

### Official EDS Documentation

Before using the aem-boilerplate, we recommend you to go through the documentation on https://www.aem.live/docs/ and more specifically:
1. [Developer Tutorial](https://www.aem.live/developer/tutorial)
2. [The Anatomy of a Project](https://www.aem.live/developer/anatomy-of-a-project)
3. [Web Performance](https://www.aem.live/developer/keeping-it-100)
4. [Markup, Sections, Blocks, and Auto Blocking](https://www.aem.live/developer/markup-sections-blocks)
5. [Block Collection](https://www.hlx.live/developer/block-collection)

## Installation

```sh
npm i
```

## Linting

```sh
npm run lint
```

## Local development

1. Create a new repository based on the `aem-boilerplate` template
1. Add the [AEM Code Sync GitHub App](https://github.com/apps/aem-code-sync) to the repository
1. Install the [AEM CLI](https://github.com/adobe/helix-cli): `npm install -g @adobe/aem-cli`
1. Start AEM Proxy: `aem up` (opens your browser at `http://localhost:3000`)
1. Open the `{repo}` directory in your favorite IDE and start coding :)
