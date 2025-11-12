# Project Context for AI Assistants

## Project Type

This is an **Adobe Experience Manager Edge Delivery Services (EDS)** project.

## Critical Content Rules

### Markdown Block Structure

**ALL content pages must use ASCII table format for blocks, NOT standard markdown tables.**

❌ **WRONG** - Standard Markdown Tables:
```markdown
| Column 1 | Column 2 |
|----------|----------|
| Data     | Data     |
```

✅ **CORRECT** - ASCII Table Format:
```
+----------+----------+
| Column 1 | Column 2 |
+----------+----------+
| Data     | Data     |
+----------+----------+
```

### Line Breaks

❌ **WRONG**: `<br>` tags
✅ **CORRECT**: `\` backslash

### Images

❌ **WRONG**: Inline `![alt](url)`
✅ **CORRECT**: References `![alt][ref]` with refs at bottom:
```
[ref]: https://example.com/image.jpg#width=750&height=500
```

## Documentation Files

When generating content for this project, ALWAYS reference these files:

1. **Quick Reference**: `/.eds-project.md` - Essential rules and examples
2. **Complete Guide**: `/docs/BLOCK-STRUCTURE.md` - Full documentation with all block types
3. **Working Examples**: `/blocks-demo.md` - Real examples of every block
4. **Command Reference**: `/.claude/commands/block-structure.md` - Quick command helper

## Available Blocks

This project has these blocks implemented in `/blocks/`:

- accordion
- cards
- carousel
- columns
- embed
- footer
- fragment
- header
- hero
- search
- table
- tabs
- video

## Block Structure Quick Reference

**Single Column (Hero, Video, Embed, Search)**:
```
+--------------------------------------------------------------------------+
| Block Name                                                               |
+--------------------------------------------------------------------------+
| Content                                                                  |
+--------------------------------------------------------------------------+
```

**Two Column (Cards, Carousel)**:
```
+--------------------------------------------------------------------------------+
| Block Name                                                                     |
+----------------------+---------------------------------------------------------+
| Left                 | Right                                                   |
+----------------------+---------------------------------------------------------+
```

**Equal Columns (Columns)**:
```
+--------------------------------------------------------------------------------------------------------------------+
| Columns                                                                                                            |
+--------------------------------------------------------+-----------------------------------------------------------+
| Left Half                                              | Right Half                                                |
+--------------------------------------------------------+-----------------------------------------------------------+
```

**Label/Content (Accordion, Tabs)**:
```
+--------------------------------------------------------------------------------+
| Block Name                                                                     |
+--------------------+-----------------------------------------------------------+
| Label              | Content                                                   |
+--------------------+-----------------------------------------------------------+
```

**Multi-Column Data (Table)**:
```
+---------------------------------------------------------------------------------+
| Table                                                                           |
+--------+--------+--------+--------+
| Col 1  | Col 2  | Col 3  | Col 4  |
+--------+--------+--------+--------+
| Data   | Data   | Data   | Data   |
+--------+--------+--------+--------+
```

## Content Generation Workflow

When asked to create a new page:

1. ✅ Read `/blocks-demo.md` for reference
2. ✅ Use ASCII table format with `+`, `-`, `|`
3. ✅ Put block name in first row
4. ✅ Use `\` for line breaks
5. ✅ Use reference-style images
6. ✅ Place image refs at bottom with dimensions
7. ✅ Separate blocks with `---`
8. ✅ Verify structure matches examples

## Common Patterns

**Hero with CTA**:
```
+--------------------------------------------------------------------------+
| Hero                                                                     |
+--------------------------------------------------------------------------+
| ![Background][img]                                                       |
+--------------------------------------------------------------------------+
| **Heading**\                                                             |
| \                                                                        |
| Description text.\                                                       |
| \                                                                        |
| [Call to Action](/)\                                                     |
| \                                                                        |
| [Secondary Action](/)                                                    |
+--------------------------------------------------------------------------+
```

**3-Column Cards**:
```
+--------------------------------------------------------------------------------+
| Cards                                                                          |
+----------------------+---------------------------------------------------------+
| ![Card 1][img1]      | **Card 1 Title**\                                       |
|                      | \                                                       |
|                      | Card 1 description.\                                    |
|                      | \                                                       |
|                      | [Learn More](/)                                         |
+----------------------+---------------------------------------------------------+
| ![Card 2][img2]      | **Card 2 Title**\                                       |
|                      | \                                                       |
|                      | Card 2 description.\                                    |
|                      | \                                                       |
|                      | [Learn More](/)                                         |
+----------------------+---------------------------------------------------------+
| ![Card 3][img3]      | **Card 3 Title**\                                       |
|                      | \                                                       |
|                      | Card 3 description.\                                    |
|                      | \                                                       |
|                      | [Learn More](/)                                         |
+----------------------+---------------------------------------------------------+
```

**FAQ Accordion**:
```
+------------------------------------------------------------------------------------------+
| Accordion                                                                                |
+------------------------------+-----------------------------------------------------------+
| Question 1?                  | Answer to question 1 with detailed explanation.           |
+------------------------------+-----------------------------------------------------------+
| Question 2?                  | Answer to question 2 with more details.                   |
+------------------------------+-----------------------------------------------------------+
```

## Image Dimension Standards

Common image dimensions used in this project:

- Hero images: `#width=2000&height=1333`
- Card images: `#width=750&height=500`
- Video thumbnails: `#width=750&height=422`
- Square images: `#width=1024&height=1024`

## Block Variants

Variants are specified by modifying the block name:

- `Hero` → `Hero Cta`, `Hero Subscribe`, `Hero Feature`
- `Cards` → `Cards Trends`, `Cards Articles`
- `Columns` → `Columns Banner`, `Columns Pictures`
- `Table` → `Table (striped)`, `Table (bordered)`, `Table (no-header)`

## Testing Generated Content

After generating content:

1. Verify ASCII table format is used
2. Check line breaks use `\` not `<br>`
3. Confirm images use references
4. Ensure image refs have dimensions
5. Compare structure to `/blocks-demo.md`

## Example Reference

See `/blocks-demo.md` - this file contains working examples of all 10+ blocks with proper formatting.

## Important Notes

- **NEVER** use standard markdown tables for blocks
- **NEVER** use `<br>` tags
- **NEVER** use inline images
- **ALWAYS** reference the documentation files listed above
- **ALWAYS** verify generated content matches `/blocks-demo.md` format

---

Last Updated: 2025-11-12
Project: EDS Block Collection Demo
