# Libertinus for Typora

A light [Typora](https://typora.io/) theme inspired by a Pandoc and XeLaTeX article set in Libertinus. Made for notes, essays, and technical writing, with a 16 cm reading measure, LaTeX-style heading sizes, booktabs-style tables, and serif fallbacks for Chinese text.

Blockquotes use italic text with a narrow grey left border; code stays upright. Click inside a code block to edit its language in the footer below the code, without scrolling to reveal the selector.

![Libertinus typography, blockquote, and table in Typora](docs/typography.png)

![Python code and a displayed equation in Typora](docs/code-and-math.png)

## Install

1. Download and unzip the [latest release](https://github.com/wei-yuhang/typora-theme-libertinus/releases/latest), or download [`libertinus.css`](libertinus.css) using GitHub’s **Download raw file** button.
2. In Typora, open **Preferences → Appearance → Open Theme Folder** and copy `libertinus.css` into that folder.
3. Restart Typora and choose **Themes → Libertinus**.

Only the CSS file belongs in the theme folder. Open [`sample.md`](sample.md) to try headings, quotations, tables, code, math, Chinese text, lists, and footnotes.

See the [Typora theme installation guide](https://theme.typora.io/doc/Install-Theme/) for platform-specific details.

## Fonts

Fonts are **not bundled**. Install Libertinus Serif and Libertinus Sans from the [official Libertinus releases](https://github.com/alerque/libertinus/releases) for the intended appearance. Open the downloaded `.otf` files with Font Book on macOS, or select them and choose **Install** on Windows, then restart Typora.

For Chinese text, the intended font is **思源宋体 (Source Han Serif)**. Install the Simplified Chinese edition from the [official Adobe font releases](https://github.com/adobe-fonts/source-han-serif/releases). The CSS looks for `Source Han Serif SC` / `Source Han Serif CN` and their Chinese names first, then Noto Serif CJK and system serif fallbacks if 思源宋体 is unavailable. Fonts are not downloaded automatically by the theme.

The theme also recognizes Libertinus Mono and Libertinus Math. Code prefers Fira Code or JetBrains Mono when installed, then falls back to Libertinus Mono and system monospace fonts. The screenshots use fonts installed on macOS, so other systems can look slightly different.

Math uses Typora’s configured renderer. Setting a CSS font family does not replace glyphs drawn as SVG by MathJax.

## Compatibility

- Used long-term on **Windows** by the author.
- Checked in **Typora 1.14.15 on macOS**, including the recent code-language picker changes, narrow editor/sidebar layout, source mode, tables, math, lists, and PDF export.
- **Linux has not been tested.**

This is a light theme, including when selected under the operating system’s dark appearance. It does not include a separate dark variant. PDF page size and physical margins are controlled by Typora’s export settings; the theme’s screen layout is inspired by A4 rather than an exact LaTeX page reproduction.

## License

The theme, sample, and screenshots are available under the [MIT License](LICENSE). Separately installed fonts retain their own licenses.
