---
description: Generate EDS content with correct block structure
---

# EDS Block Structure Command

When generating markdown content for this EDS project, ALWAYS follow these rules:

## Block Format

Use ASCII tables with borders for ALL blocks:

```
+--------------------------------------------------------------------------+
| Block Name                                                               |
+--------------------------------------------------------------------------+
| Content                                                                  |
+--------------------------------------------------------------------------+
```

## Key Rules

1. **Tables**: Use `+`, `-`, `|` characters (NOT markdown tables)
2. **Line breaks**: Use `\` backslash (NOT `<br>`)
3. **Images**: Use `![alt][ref]` references (NOT inline)
4. **Image refs**: At bottom with dimensions: `[ref]: url#width=750&height=500`

## Quick Examples

**Hero**:
```
+--------------------------------------------------------------------------+
| Hero                                                                     |
+--------------------------------------------------------------------------+
| ![Background][img]                                                       |
+--------------------------------------------------------------------------+
| **Title**\                                                               |
| \                                                                        |
| Description\                                                             |
| \                                                                        |
| [CTA](/)                                                                 |
+--------------------------------------------------------------------------+
```

**Cards**:
```
+--------------------------------------------------------------------------------+
| Cards                                                                          |
+----------------------+---------------------------------------------------------+
| ![Image][img1]       | **Title**\                                              |
|                      | \                                                       |
|                      | Description\                                            |
|                      | \                                                       |
|                      | [Link](/)                                               |
+----------------------+---------------------------------------------------------+
```

**Columns**:
```
+--------------------------------------------------------------------------------------------------------------------+
| Columns                                                                                                            |
+--------------------------------------------------------+-----------------------------------------------------------+
| **Left**\                                              | **Right**\                                                |
| \                                                      | \                                                         |
| Content                                                | Content                                                   |
+--------------------------------------------------------+-----------------------------------------------------------+
```

## Reference Files

- Complete guide: `/docs/BLOCK-STRUCTURE.md`
- Working examples: `/blocks-demo.md`
- Quick reference: `/.eds-project.md`

## Available Blocks

accordion, cards, carousel, columns, embed, footer, fragment, header, hero, search, table, tabs, video

ALWAYS verify generated content matches the format in `/blocks-demo.md`
