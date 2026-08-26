# Jameel Noori Nastaliq — Discourse Theme Component

A Discourse theme component that adds **Jameel Noori Nastaliq** as a site-wide font, with support for both Regular and Bold font weights.

The component is particularly suitable for Urdu and other multilingual Discourse communities where a friendly, readable typeface is desired.

## Features

* Adds **Jameel Noori Nastaliq** as the primary font.
* Applies the font throughout the Discourse interface.
* Enables normal font ligatures.
* Includes the original font files locally, so the component does not depend on an external font CDN.
* Works with both light and dark Discourse themes.

## Installation

In your Discourse administrator interface:

1. Go to **Appearance → Themes & Components** then click Components.

2. Click install a new theme component from **⋮**.

4. Select **Install via Git repository**.

5. Enter:

   `https://github.com/mfgbhatti/JameelNooriNastaliq.git`

   6. Install the component.

   7. Add the component to your active theme.

   After installation, rebuild the theme if necessary and reload your Discourse site.

   ## Font Variants

   The component includes two font files:

   | Font                     | Weight | Type     |
   | ------------------------ | ------ | ----------- |
   | JameelNooriNastaliq.ttf | 400    | ttf |
   | JameelNooriNastaliq.woff2 | 400    | WOFF2    |

   The Regular font `JameelNooriNastaliq.woff2` is exposed as `JameelNooriNastaliqWeb`, while the `JameelNooriNastaliq.ttf` font not exposed as `JameelNooriNastaliqTrue`.

   ## How It Works

   The font files are declared using CSS `@font-face` rules and then assigned to Discourse's global font variables.

   Regular text uses:

   `JameelNooriNastaliqWeb, Arial, sans-serif`

   other use:

   `JameelNooriNastaliqTrue, Arial, sans-serif`

   The component also enables normal font ligatures for the document and headings.

   ## Files

   ```text
   JameelNooriNastaliq/
   ├── assets/
   │   ├── JameelNooriNastaliq.ttf
   │   ├── JameelNooriNastaliq.woff2
   ├── common/
   │   └── common.scss
   ├── about.json
   ├── LICENSE
   └── README.md
   ```

   The font assets are referenced by `about.json`, which maps the Regular and Bold font files to the component's asset variables.

   ## License

   This repository contains the Discourse theme component code as well as font files distributed under their respective licenses.

   The repository's theme component code is licensed under the **MIT License**. Please see [`LICENSE`](LICENSE) for the complete license text.

   Please retain these files when redistributing the font assets.

   ## Credits

   * **Jameel Noori Nastaliq** — font

   ## Repository

   Source code and updates:
   ```bash

   https://github.com/mfgbhatti/JameelNooriNastaliq.git
   ```

   ## Contributing

   Issues, suggestions, and pull requests are welcome.

   If you find a problem with the font rendering or compatibility with a newer Discourse version, please open an issue in the repository.

   ## Disclaimer

    - This project is an independent Discourse theme component and is not affiliated with or endorsed by Discourse or the Jameel Noori Nastaliq font authors.
