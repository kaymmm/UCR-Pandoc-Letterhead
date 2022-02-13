# UCR-Pandoc-Letterhead-2020

Unofficial copy of UCR Letterhead for Pandoc based on 2020 UCR Brand Identity

Based on the UCR Visual Identity Guidelines 2020

Forked from the homie Flip Tanedo <https://github.com/fliptanedo/UCR-XeLaTeX-Letterhead-2020>

Demo: [Test Letter PDF](https://github.com/kaymmm/UCR-Pandoc-Letterhead/blob/master/test_letter.pdf)

## Requirements

* Rift font: https://www.dafontfree.io/download/rift/
* EB Garamond: available free on Google fonts
* Oswald and Fira Sans are acceptable substitutions, when Rift or EB Garamond is unavailable . Both are also available from the Google fonts repository.
* Pandoc w/XeLaTeX or LuaLaTeX to compile (not PdfLaTeX)
* LuaLaTeX if you want to use fallback fonts for unavailable glyphs

## Usage

REQUIRED:

* Pandoc w/XeLaTeX or LuaLaTeX
* Rift font: https://www.dafontfree.io/download/rift/
* EB Garamond font (Google Fonts)
* Fira Sans font (Google Fonts)
* Oswald font (fallback)

Create your letter in a Pandoc-compatible format. It should include the opening salutation and body text only. Everything else is set using Pandoc parameters.

Mandatory or recommended* Pandoc parameters:

* author
* position (your title)
* department
* recipient* (array; each line of recipient inside address)
* secondary-style* (bool; use secondary version letterhead)
* signature-image
* address* (array; each line of address)
* phone*
* email*
* website*
* lang* (probably helpful for hyphenation)

Optional Pandoc parameters:

* date
* indent (bool)
* left-align (bool; otherwise justify)
* gray-seal (bool; use gray watermark instead of yellow)
* address-rgb (list of 3 RGB values 0-255 to use for header/footer text)
* Custom Fonts: (must include options for size, letter spacing, etc. if specified)
  * headerfont (font name, suggested Rift [default] or Oswald)
  * footerfont (font name, suggested Rift [default] or Oswald)
  * sansfont (font name, Fira Sans is default)
  * mainfont (font name, EB Garamond is default)
* sansbody (bool) [use sans font for body]
* fallback-fonts (list of fallback fonts for glyphs not in the main font)
* many of the other standard Pandoc options


## TO-DO:

* [ ] Adjust positionings to use papersize
* [ ] Pull in other Pandoc options where useful, e.g., CJK fonts
* [ ] Greater flexibility with line and font spacing
* [ ] Adjustable indents, including first paragraph after section heading
* [ ] Testing across the board
* [ ] Pull out extraneous stuff pulled in from Pandoc


## Disclaimer

Neither I nor Flip Tanedo take responsibility for how you use this template.

## License

Logos property of UCR.

Per the UCR Brand Identity website: "Unauthorized, unaffiliated, or personal websites, publications, channels, print and/or digital materials are not allowed to use/feature UCR institutional logos without the express written permission of University Communications."

Pandoc template (c) 2022 Keith Miyake

Original Latex template (c) 2020–2022 Flip Tanedo

Code contributed by Keith Miyake licensed GPLv3 (see LICENSE)
