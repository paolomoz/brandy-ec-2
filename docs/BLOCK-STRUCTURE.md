# EDS Block Structure Guide

This document defines the correct markdown structure for creating EDS blocks in this project. **All content pages must follow these patterns.**

## Table of Contents

1. [General Rules](#general-rules)
2. [Block Table Format](#block-table-format)
3. [Block Examples](#block-examples)
4. [Image References](#image-references)

---

## General Rules

### Basic Syntax

- Blocks use **ASCII table format** with `+`, `-`, and `|` characters
- Block names go in the **first row** of each table
- Use `\` (backslash) for **line breaks** within cells
- Separate blocks with `---` (horizontal rule)
- Image references go at the **bottom of the file**

### Line Breaks in Cells

```
| **Heading**\                          |
| \                                     |
| First paragraph text.\                |
| \                                     |
| Second paragraph text.                |
```

### Links and Images

- Links: `[Link Text](/path)`
- Images: `![Alt Text][image-ref]`
- Image references at bottom: `[image-ref]: https://example.com/image.jpg#width=750&height=500`

---

## Block Table Format

### Single Column Block

```
+--------------------------------------------------------------------------+
| Block Name                                                               |
+--------------------------------------------------------------------------+
| Content goes here                                                        |
+--------------------------------------------------------------------------+
```

### Two Column Block

```
+--------------------------------------------------------------------------------+
| Block Name                                                                     |
+----------------------+---------------------------------------------------------+
| Left Column          | Right Column                                            |
+----------------------+---------------------------------------------------------+
```

### Multi-Row Two Column

```
+--------------------------------------------------------------------------------+
| Block Name                                                                     |
+----------------------+---------------------------------------------------------+
| Row 1 Left           | Row 1 Right                                             |
+----------------------+---------------------------------------------------------+
| Row 2 Left           | Row 2 Right                                             |
+----------------------+---------------------------------------------------------+
```

### Three Column Block

```
+-----------------------------------------------------------------------+
| Block Name                                                            |
+---------------------+----------------------+----------------------+
| Column 1            | Column 2             | Column 3             |
+---------------------+----------------------+----------------------+
```

### Multi-Column Data Table

```
+---------------------------------------------------------------------------------+
| Table                                                                           |
+-------------+-----------------------------------+-----------+---------------------+
| Header 1    | Header 2                          | Header 3  | Header 4            |
+-------------+-----------------------------------+-----------+---------------------+
| Data 1      | Data 2                            | Data 3    | Data 4              |
+-------------+-----------------------------------+-----------+---------------------+
```

---

## Block Examples

### Hero Block

```
+--------------------------------------------------------------------------+
| Hero                                                                     |
+--------------------------------------------------------------------------+
| ![Hero Background][hero-img]                                             |
+--------------------------------------------------------------------------+
| **Welcome to Our Site**\                                                 |
| \                                                                        |
| Explore amazing content and discover new possibilities.\ \               |
| [Get Started](/)\                                                        |
| \                                                                        |
| [Learn More](/)                                                          |
+--------------------------------------------------------------------------+
```

### Cards Block

```
+--------------------------------------------------------------------------------+
| Cards                                                                          |
+----------------------+---------------------------------------------------------+
| ![Card 1][card1-img] | **Card Title**\                                         |
|                      | \                                                       |
|                      | Card description text goes here.\                       |
|                      | \                                                       |
|                      | [Learn More](/)                                         |
+----------------------+---------------------------------------------------------+
| ![Card 2][card2-img] | **Another Card**\                                       |
|                      | \                                                       |
|                      | More card content.\                                     |
|                      | \                                                       |
|                      | [Learn More](/)                                         |
+----------------------+---------------------------------------------------------+
```

### Columns Block

```
+--------------------------------------------------------------------------------------------------------------------+
| Columns                                                                                                            |
+--------------------------------------------------------+-----------------------------------------------------------+
| **Left Column Heading**\                               | **Right Column Heading**\                                 |
| \                                                      | \                                                         |
| Content for the left column goes here. Can be          | Content for the right column. Can include multiple        |
| multiple lines and paragraphs.                         | paragraphs as well.                                       |
+--------------------------------------------------------+-----------------------------------------------------------+
```

### Columns with Image and Text

```
+--------------------------------------------------------------------------------------------------------------------+
| Columns                                                                                                            |
+--------------------------------------------------------+-----------------------------------------------------------+
| ![Image][img1]                                         | **Feature Title**\                                        |
|                                                        | \                                                         |
|                                                        | Description text for this feature goes here.              |
+--------------------------------------------------------+-----------------------------------------------------------+
| **Another Feature**\                                   | ![Image][img2]                                            |
| \                                                      |                                                           |
| Text on the left, image on the right.                  |                                                           |
+--------------------------------------------------------+-----------------------------------------------------------+
```

### Accordion Block

```
+------------------------------------------------------------------------------------------+
| Accordion                                                                                |
+------------------------------+-----------------------------------------------------------+
| Question or heading?         | Answer or content goes here. Can be multiple lines and    |
|                              | wrap across the cell.                                     |
+------------------------------+-----------------------------------------------------------+
| Another question?            | Another answer with detailed explanation.                 |
+------------------------------+-----------------------------------------------------------+
```

### Tabs Block

```
+--------------------------------------------------------------------------------+
| Tabs                                                                           |
+--------------------+-----------------------------------------------------------+
| Tab 1 Label        | **Tab 1 Content Heading**\                                |
|                    | \                                                         |
|                    | Content for the first tab. Can include multiple lines and |
|                    | paragraphs.                                               |
+--------------------+-----------------------------------------------------------+
| Tab 2 Label        | **Tab 2 Content Heading**\                                |
|                    | \                                                         |
|                    | Content for the second tab.                               |
+--------------------+-----------------------------------------------------------+
```

### Table Block

```
+---------------------------------------------------------------------------------+
| Table                                                                           |
+-------------+-----------------------------------+-----------+---------------------+
| Column 1    | Column 2                          | Column 3  | Column 4            |
+-------------+-----------------------------------+-----------+---------------------+
| Data 1      | Data 2                            | Data 3    | Data 4              |
+-------------+-----------------------------------+-----------+---------------------+
| More data   | Additional information            | Value     | Another value       |
+-------------+-----------------------------------+-----------+---------------------+
```

### Video Block

```
+--------------------------------------------------------------------------------+
| Video                                                                          |
+--------------------------------------------------------------------------------+
| ![Video Thumbnail][video-img]                                                  |
+--------------------------------------------------------------------------------+
| https://www.youtube.com/watch?v=VIDEO_ID                                       |
+--------------------------------------------------------------------------------+
```

### Carousel Block

```
+--------------------------------------------------------------------------------+
| Carousel                                                                       |
+----------------------+---------------------------------------------------------+
| ![Slide 1][slide1]   | **Slide Title**\                                        |
|                      | \                                                       |
|                      | Description for this slide.                             |
+----------------------+---------------------------------------------------------+
| ![Slide 2][slide2]   | **Another Slide**\                                      |
|                      | \                                                       |
|                      | More slide content.                                     |
+----------------------+---------------------------------------------------------+
```

### Embed Block

```
+--------------------------------------------------------------------------------+
| Embed                                                                          |
+--------------------------------------------------------------------------------+
| ![Embed Placeholder][embed-img]                                                |
+--------------------------------------------------------------------------------+
| https://www.youtube.com/watch?v=VIDEO_ID                                       |
+--------------------------------------------------------------------------------+
```

### Search Block

```
+--------------------------------------------------------------------------------+
| Search                                                                         |
+--------------------------------------------------------------------------------+
| [/query-index.json](/)                                                         |
+--------------------------------------------------------------------------------+
```

### Fragment Block

```
+------------------------------+
| Fragment                     |
+------------------------------+
| [/fragments/header](/)       |
+------------------------------+
```

---

## Image References

Always place image references at the **bottom of the markdown file**:

```markdown
[hero-img]: https://example.com/image.jpg#width=2000&height=1333
[card1-img]: https://example.com/card1.jpg#width=750&height=500
[card2-img]: https://example.com/card2.jpg#width=750&height=500
[video-img]: https://example.com/video-thumb.jpg#width=750&height=422
```

### Image Dimensions

Common image dimension patterns:

- **Hero images**: `#width=2000&height=1333`
- **Card images**: `#width=750&height=500`
- **Video thumbnails**: `#width=750&height=422`
- **Square images**: `#width=1024&height=1024`

---

## Block Variants

To apply a variant to a block, add the variant name to the block header row:

```
+--------------------------------------------------------------------------+
| Hero Cta                                                                 |
+--------------------------------------------------------------------------+
```

```
+--------------------------------------------------------------------------+
| Cards Trends                                                             |
+--------------------------------------------------------------------------+
```

```
+--------------------------------------------------------------------------+
| Table (striped)                                                          |
+--------------------------------------------------------------------------+
```

Common variants:
- Hero: `Hero`, `Hero Cta`, `Hero Subscribe`, `Hero Feature`
- Cards: `Cards`, `Cards Trends`, `Cards Articles`
- Columns: `Columns`, `Columns Banner`, `Columns Pictures`
- Table: `Table`, `Table (striped)`, `Table (bordered)`, `Table (no-header)`

---

## Complete Page Example

```markdown
# Page Title

Brief page description.

---

+--------------------------------------------------------------------------+
| Hero                                                                     |
+--------------------------------------------------------------------------+
| ![Hero Background][hero-img]                                             |
+--------------------------------------------------------------------------+
| **Page Heading**\                                                        |
| \                                                                        |
| Descriptive text.\                                                       |
| \                                                                        |
| [CTA Button](/)                                                          |
+--------------------------------------------------------------------------+

---

+--------------------------------------------------------------------------------------------------------------------+
| Columns                                                                                                            |
+--------------------------------------------------------+-----------------------------------------------------------+
| **Feature 1**\                                         | **Feature 2**\                                            |
| \                                                      | \                                                         |
| Feature description.                                   | Another feature description.                              |
+--------------------------------------------------------+-----------------------------------------------------------+

---

+--------------------------------------------------------------------------------+
| Cards                                                                          |
+----------------------+---------------------------------------------------------+
| ![Card][card-img]    | **Card Title**\                                         |
|                      | \                                                       |
|                      | Card content.\                                          |
|                      | \                                                       |
|                      | [Read More](/)                                          |
+----------------------+---------------------------------------------------------+

---

## Additional Content

Regular markdown content can go between blocks.

[hero-img]: https://example.com/hero.jpg#width=2000&height=1333
[card-img]: https://example.com/card.jpg#width=750&height=500
```

---

## Common Mistakes to Avoid

❌ **Wrong**: Using simple markdown tables
```markdown
| Column 1 | Column 2 |
|----------|----------|
| Data     | Data     |
```

✅ **Correct**: Using ASCII table format
```
+----------+----------+
| Column 1 | Column 2 |
+----------+----------+
| Data     | Data     |
+----------+----------+
```

❌ **Wrong**: Using `<br>` for line breaks
```
**Heading**<br>
Content here
```

✅ **Correct**: Using backslash `\` for line breaks
```
**Heading**\
\
Content here
```

❌ **Wrong**: Inline images
```markdown
![Image](https://example.com/image.jpg)
```

✅ **Correct**: Reference-style images
```markdown
![Image][img-ref]

[img-ref]: https://example.com/image.jpg#width=750&height=500
```

---

## Quick Reference Checklist

When creating a new content page:

- [ ] Use ASCII table format with `+`, `-`, `|`
- [ ] Put block name in first row
- [ ] Use `\` for line breaks within cells
- [ ] Separate blocks with `---`
- [ ] Use reference-style images
- [ ] Place image references at bottom of file
- [ ] Include width and height in image URLs
- [ ] Test rendering in preview environment

---

## Additional Resources

- [Official EDS Documentation](https://www.hlx.live/developer/block-collection)
- [Block Collection Catalog](https://www.hlx.live/developer/block-collection)
- Example: `/blocks-demo.md` in this project

---

**Last Updated**: 2025-11-12
**Maintained By**: Development Team
