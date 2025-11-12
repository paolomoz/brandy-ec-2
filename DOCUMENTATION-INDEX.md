# Documentation Index

This document serves as the central index for all project documentation.

## Quick Start

For AI assistants and developers generating content for this project:

1. **Start Here**: [PROJECT-CONTEXT.md](PROJECT-CONTEXT.md) - Essential overview
2. **Complete Reference**: [docs/BLOCK-STRUCTURE.md](docs/BLOCK-STRUCTURE.md) - Full guide
3. **Working Examples**: [blocks-demo.md](blocks-demo.md) - Live examples
4. **Quick Reference**: [.eds-project.md](.eds-project.md) - Quick lookup

## Documentation Files

### Primary Documentation

| File | Purpose | When to Use |
|------|---------|-------------|
| `PROJECT-CONTEXT.md` | High-level project overview and AI instructions | First read for understanding project type |
| `.eds-project.md` | Quick reference with block syntax | Quick lookup during content creation |
| `docs/BLOCK-STRUCTURE.md` | Complete guide with all block types | Detailed reference when creating new blocks |
| `blocks-demo.md` | Working examples of all blocks | Template/reference for specific block types |

### Helper Files

| File | Purpose |
|------|---------|
| `.claude/commands/block-structure.md` | Claude Code command reference |
| `README.md` | Updated with block list and documentation links |
| `DOCUMENTATION-INDEX.md` | This file - documentation overview |

## EDS Block Structure Rules

**Critical**: All content must use ASCII table format for blocks.

### Correct Format

```
+--------------------------------------------------------------------------+
| Block Name                                                               |
+--------------------------------------------------------------------------+
| Content with backslash for line breaks\                                  |
| \                                                                        |
| More content                                                             |
+--------------------------------------------------------------------------+
```

### DO NOT Use

- ❌ Standard markdown tables (`| col |`)
- ❌ HTML `<br>` tags
- ❌ Inline images `![alt](url)`

### DO Use

- ✅ ASCII tables with `+`, `-`, `|`
- ✅ Backslash `\` for line breaks
- ✅ Reference images `![alt][ref]` with refs at bottom

## Available Blocks

All blocks are implemented in `/blocks/` directory:

1. **accordion** - FAQ/expandable sections
2. **cards** - Card grid layouts
3. **carousel** - Image sliders
4. **columns** - Multi-column layouts
5. **embed** - External content embeds
6. **footer** - Site footer
7. **fragment** - Reusable fragments
8. **header** - Site header
9. **hero** - Hero sections
10. **search** - Search functionality
11. **table** - Data tables
12. **tabs** - Tabbed interfaces
13. **video** - Video embeds

## Content Creation Workflow

When creating a new page:

1. ✅ Reference `blocks-demo.md` for the specific block type
2. ✅ Copy the ASCII table structure
3. ✅ Use `\` for line breaks within cells
4. ✅ Use reference-style images
5. ✅ Add image refs at bottom with dimensions
6. ✅ Separate blocks with `---`
7. ✅ Verify format matches examples

## Common Block Patterns

See each documentation file for detailed examples:

- **Hero**: Single column with image, heading, text, CTAs
- **Cards**: Two columns (image + content) repeated for each card
- **Columns**: Equal width columns for feature comparisons
- **Accordion**: Two columns (question + answer)
- **Tabs**: Two columns (tab label + tab content)
- **Table**: Multi-column data with headers
- **Video/Embed**: Single column with thumbnail + URL
- **Carousel**: Two columns (image + content) for each slide
- **Search**: Single column with data source link

## Image Guidelines

Images should include dimensions:

```markdown
[img-ref]: https://example.com/image.jpg#width=750&height=500
```

Common dimensions:
- Hero: `width=2000&height=1333`
- Cards: `width=750&height=500`
- Video: `width=750&height=422`
- Square: `width=1024&height=1024`

## Testing Your Content

Before committing:

1. Compare structure to `blocks-demo.md`
2. Verify ASCII table format (not markdown tables)
3. Check line breaks use `\`
4. Confirm images are references, not inline
5. Test in preview environment

## Getting Help

- Examples: See `blocks-demo.md`
- Full guide: See `docs/BLOCK-STRUCTURE.md`
- Quick reference: See `.eds-project.md`
- AI context: See `PROJECT-CONTEXT.md`

## File Locations

```
.
├── PROJECT-CONTEXT.md          # AI assistant instructions
├── .eds-project.md             # Quick reference guide
├── blocks-demo.md              # Working examples
├── DOCUMENTATION-INDEX.md      # This file
├── README.md                   # Project readme (updated)
├── docs/
│   └── BLOCK-STRUCTURE.md      # Complete documentation
├── .claude/
│   └── commands/
│       └── block-structure.md  # Claude Code command
└── blocks/                     # Block implementations
    ├── accordion/
    ├── cards/
    ├── carousel/
    ├── columns/
    ├── embed/
    ├── footer/
    ├── fragment/
    ├── header/
    ├── hero/
    ├── search/
    ├── table/
    ├── tabs/
    └── video/
```

---

**Last Updated**: 2025-11-12  
**Project Type**: Adobe EDS (Edge Delivery Services)  
**Purpose**: Block collection demonstration and reference
