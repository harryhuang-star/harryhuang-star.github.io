# Mushoku Tensei blog — TGJ3M Assignment 2

A blog about the anime **Mushoku Tensei: Jobless Reincarnation**, built using only the
HTML and CSS from the Unit 1 review sheet.

Author: **Harry** · just under 200 lines of HTML and CSS in total.

| File | What it is |
|---|---|
| `index.html` | About Me — this is what opens when you visit the site |
| `home.html` | The main page of the blog |
| `post.html` | The blog post about Mushoku Tensei |
| `a5.html` | The A5 page — the movie poster, shown at full width |
| `styles.css` | The stylesheet, linked from every page |
| `images/` | The 5 pictures, plus the A5 poster |

## Open it in VS Code

**File › Open Folder…** → pick this folder, then open `index.html` for the About Me page.
The main page is `home.html`, the blog post is `post.html` and the poster page is `a5.html`.
(With the **Live Server** extension: right-click `index.html` → Open with Live Server.)

## Everything used comes from the review sheet

**HTML elements** — nothing else appears in the files:

| Element | Where it is used |
|---|---|
| `<!DOCTYPE html>`, `<html lang="en">` | Top of both pages |
| `<head>`, `<title>` | Top of both pages |
| `<link rel="stylesheet">` | Connects `styles.css` |
| `<body>` | Page content |
| `<h1>` | The name of the blog, in the header |
| `<h2>` | The post title and the main sections |
| `<h3>` | Section headings |
| `<h4>` | The name of each character |
| `<p>` | All paragraphs and source lines |
| `<a href="...">` | `home.html` and the outside links |
| `<img src="..." alt="...">` | The 5 pictures |

**CSS** — element selectors only (`body`, `h1`, `h2`, `h3`, `h4`, `p`, `a`, `img`), and
only properties from the eight things the sheet says CSS can control:

| Sheet says CSS controls | Properties used |
|---|---|
| Colour | `color` |
| Fonts | `font-family` |
| Text size | `font-size` |
| Spacing | `margin`, `padding`, `padding-bottom` |
| Borders | `border`, `border-bottom` |
| Backgrounds | `background-color` |
| Alignment | `text-align` |
| Page layout | `max-width`, `width` |

No classes, no `div`, no flexbox or grid, no `@media`, no CSS variables, no pseudo-classes.

### Two small things to know about

1. **`<meta charset="utf-8">` and `<meta name="viewport">`** are the first two lines in
   `<head>`. The sheet's example doesn't show them, but VS Code puts them in by default
   when you type `!` and press Tab. The charset is what lets the Japanese title 無職転生
   show up correctly. If the teacher would rather they weren't there, delete those 2 lines.
2. **`line-height: 1.7`** in the `body` rule is line spacing. I counted it under
   "Spacing" on the sheet. It is one line — delete it if it isn't wanted.

## Colours and contrast

Five colours, taken from the anime's own artwork:

| Colour | Hex | Where it came from |
|---|---|---|
| Navy | `#16244A` | The night sky in the key visual |
| Gold | `#F2B233` | The gold lettering in the title logo |
| Cyan | `#6FC9E8` | The glow around the magic staff |
| Cream | `#F5F1E6` | The wheat fields and pale stone |
| Black | `#1A1C22` | The black brush lettering of the logo |

`#7A4E06` is a darker gold used only for links, so that they are dark enough to read on
the cream background. Every colour pair was measured: the lowest contrast on the page is
**6.37:1** and the highest is **15.09:1**, well over the 4.5:1 that is needed.

## Accessibility

- All 5 images have real `alt` text that describes the picture.
- Headings go h1 → h2 → h3 → h4 with no level skipped.
- Body text is 18px.
- Links are underlined (that is the browser default), so colour is not the only clue.
- Every link says where it goes — there is no "click here".

## Pictures

From the official anime website (mushokutensei.jp).
© Rifujin na Magonote / Shirotaka / Mushoku Tensei Production Committee.
Used for a school project.
