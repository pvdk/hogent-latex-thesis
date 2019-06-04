# HoGent LaTeX thesis
> Unofficial University College Ghent (HoGent) LaTeX thesis template

An unofficial [LaTeX][latex] template for dissertations/theses of students of the University College Ghent (HoGent).
Based on the TU Delft [LaTeX template][tudelft] for reports and theses.

Another, more official one is available at [this repository][hogenttin].
I choose to write my own is because that template is made for the faculty of Business and Information Management, more specifically for theses written to obtain a Bachelor of Applied Computer Science degree. Another reason is because I do not like the style of the template it was based on (The Legrand Orange Book).

# Features

- Supports both LaTex/PDFLaTeX and XeLaTeX/LuaLaTeX (recommended)
- Multilingual (Dutch and English), with sources and documentation written in English
- Native (fontenc) font support and OpenType fonts (fontspec)
- Colored titles and headings based on the faculty color
- High resolution HoGent logo as EPS/PDF
- Option to suppress colors for black/white printing
- Code highlighting with [Minted][minted]

## Fonts
All text in this thesis template is supposed to be _sans serif_. Headings, titles and text body are rendered in the excellent [Montserrat][montserrat] typeface designed by Julieta Ulanovsky. This is also the official font specified in the HoGent styling guide and the font used for the HoGent logo. On the titlepage the title is rendered with thickness _black_, the (optional) subtitle is rendered in _extra bold_.

Typewriter style text (such as source code) is displayed using the [Inconsolata][inconsolata] font created by Raph Levien. Inconsolata was chosen because it has received favorable reviews from many programmers, who consider it to be a highly readable and clear monospaced font. For extra readability of source code the following options are chosen for this font: zeros are rendered as _slashed_ and _straight quotes_ instead of curly ones.

Math text is rendered using the [FiraMath][firamath] font, a sans-serif font with Unicode math support by Xiangdong Zeng. When compiling with LaTeX/PDFLaTeX _sfmath_ is loaded instead.

All fonts come shipped with this template, but first it will see if the fonts are available on your system. Native font rendering when compiling with XeLaTeX and LuaLaTeX can be forced with the option `nativefonts`.

# Dependencies
### Windows
Please refer to [this guide][ibmguide] for installing TeX Live on Windows.

### MacOS
Please take a look at [this page][mactex] for an up-to-date version of MacTex.

### Linux
Installing the following packages on Debian/Ubuntu-based systems will cover all the package dependencies of this template:
- texlive-base
- texlive-latex-base
- texlive-latex-recommended
- texlive-bibtex-extra
- texlive-pictures
- texlive-fonts-recommended

For other Linux distros I have provided a complete list of the CTAN packages that are loaded by this template. In the second column is the Debian/Ubuntu package that contains it. Oftentimes other distros will follow the same naming scheme. If that's not the case you can search for the right package using the CTAN package name.
<details>
<summary>Click to expand</summary>

| CTAN Package  | Debian/Ubuntu |
| ------------- | ------------- |
|xkeyval|texlive-latex-recommended|
|iflang|texlive-latex-base|
|infwarerr|texlive-latex-base|
|pdftexcmds|texlive-latex-base|
|ifluatex|texlive-base|
|ltxcmds|texlive-latex-base|
|ifpdf|texlive-latex-base|
|amsmath|texlive-latex-base|
|amstext|texlive-latex-base|
|amsgen|texlive-latex-base|
|amsbsy|texlive-latex-base|
|amsopn|texlive-latex-base|
|amssymb|texlive-base|
|amsfonts|texlive-base|
|babel|texlive-latex-base|
|biblatex|texlive-bibtex-extra|
|etoolbox|texlive-latex-recommended|
|kvoptions|texlive-latex-base|
|kvsetkeys|texlive-latex-base|
|etexcmds|texlive-latex-base|
|logreq|texlive-bibtex-extra|
|ifthen|texlive-latex-base|
|url|texlive-latex-base|
|caption|texlive-latex-recommended|
|caption3|texlive-latex-recommended|
|footmisc|texlive-latex-extra|
|ifxetex|texlive-base|
|geometry|texlive-latex-base|
|ifvtex|texlive-latex-base|
|graphicx|texlive-latex-base|
|graphics|texlive-latex-base|
|trig|texlive-latex-base|
|hyperref|texlive-latex-base|
|hobsub-hyperref|texlive-latex-base|
|hobsub-generic|texlive-latex-base|
|hobsub|texlive-latex-base|
|intcalc|texlive-latex-base|
|kvdefinekeys|texlive-latex-base|
|pdfescape|texlive-latex-base|
|bigintcalc|texlive-latex-base|
|bitset|texlive-latex-base|
|uniquecounter|texlive-latex-base|
|letltxmacro|texlive-latex-base|
|hopatch|texlive-latex-base|
|xcolor-patch|texlive-latex-base|
|atveryend|texlive-latex-base|
|atbegshi|texlive-latex-base|
|refcount|texlive-latex-base|
|hycolor|texlive-latex-base|
|auxhook|texlive-latex-base|
|rerunfilecheck|texlive-latex-base|
|xcolor|texlive-latex-recommended|
|colortbl|texlive-latex-base|
|array|texlive-latex-base|
|tikz|texlive-pictures|
|pgfrcs|texlive-pictures|
|everyshi|texlive-latex-recommended|
|pgfcore|texlive-pictures|
|pgfsys|texlive-pictures|
|pgfcomp|texlive-pictures|
|pgffor|texlive-pictures|
|pgfkeys|texlive-pictures|
|pgfmath|texlive-pictures|
|titlesec|texlive-latex-extra|
|titletoc|texlive-latex-extra|
|tocbibind|texlive-latex-extra|
|fancyhdr|texlive-latex-base|
|montserrat|texlive-fonts-extra|
|textcomp|texlive-latex-base|
|mweights|texlive-fonts-extra|
|fontaxes|texlive-latex-extra|
|inconsolata|texlive-fonts-extra|
|sfmath|texlive-latex-extra|
|fontenc|texlive-latex-base|
|snapshot|texlive-latex-extra|
|epsfig|texlive-latex-base|
|makeidx|texlive-latex-base|
|xspace|texlive-latex-base|
|listings|texlive-latex-recommended|
|lstmisc|texlive-latex-recommended|
|microtype|texlive-latex-recommended|
|minted|texlive-latex-extra|
|fvextra|texlive-latex-extra|
|fancyvrb|texlive-latex-recommended|
|upquote|texlive-latex-extra|
|lineno|texlive-latex-recommended|
|calc|texlive-latex-base|
|shellesc|texlive-latex-base|
|ifplatform|texlive-latex-extra|
|catchfile|texlive-latex-base|
|xstring|texlive-latex-extra|
|framed|texlive-latex-extra|
|float|texlive-latex-recommended|
|csquotes|texlive-latex-extra|
|eurosym|texlive-fonts-recommended|
|pdfpages|texlive-latex-recommended|
|eso-pic|texlive-latex-recommended|
|standalone|texlive-latex-extra|
|currfile|texlive-latex-extra|
|filehook|texlive-latex-recommended|
|gincltex|texlive-pictures|
|svn-prov|texlive-latex-extra|
|adjustbox|texlive-latex-extra|
|adjcalc|texlive-latex-extra|
|trimclip|texlive-latex-extra|
|collectbox|texlive-latex-extra|
|ifoddpage|texlive-latex-extra|
|varwidth|texlive-latex-extra|
|filemod-expmin|texlive-latex-extra|
|wrapfig|texlive-latex-extra|
|enumitem|texlive-latex-extra|
|tcolorbox|texlive-latex-extra|
|verbatim|texlive-latex-base|
|environ|texlive-latex-extra|
|trimspaces|texlive-latex-extra|
|tabularx|texlive-latex-base|
|booktabs|texlive-latex-recommended|
|rotating|texlive-latex-base|
|makecell|texlive-latex-extra|
|epstopdf-base|texlive-latex-base|
|grfext|texlive-latex-base|
|nameref|texlive-latex-base|
|gettitlestring|texlive-latex-base|
|pdflscape|texlive-latex-base|
|lscape|texlive-latex-base|

</details>

## Installation
You can clone this repository using git, but it might be better to download it as a ZIP and extract it. That way you will not get the whole history tree. To do this press the green _Clone or download_ button in the upper right corner of [this page][www].

## Getting started
The title and chapter headings are rendered in the color of your faculty. The color gets set by adding the faculty to the class options in [thesis\.tex][thesistex]:
```latex
\documentclass[table,twoside,english,fbo]{hogentthesis}
```
In the example above the faculty is set to `fbo` which is the abbreviation of the faculty of Business and Information Management (Faculteit Bedrijf en Organisatie). Other valid options are:
- `fmw` for the faculty of Education, Health and Social Work (Faculteit Mens en Organisatie)
- `fnt` for the Faculty of Science and Technology (Faculteit Natuur en Techniek)
- `soa` for the School of Arts, Royal Academy of Fine Arts (KASK) and the Royal Conservatory (Koninklijk Conservatorium)

## Code highlighting with Minted
Realistically the only people at the HoGent that _might_ use this template are students and faculty members of the faculty of Business and Information Management. Therefore support for code highlighting is included. An example implementation for displaying external Java code is provided, see [thesis.tex][thesistex] for the macro.

It is called like this:
```latex
\javacode{sample/binaryconverter.java}
```
and it looks like this:

![Minted](https://raw.githubusercontent.com/pvdk/hogent-latex-thesis/master/minted.png?raw=true)

### Getting it to work
To get syntax highlighting to work in LaTeX the Python package [Pygments][pygments] needs to be installed. In order to do this you can do a `pip install Pygments` or use your distro's package manager if you're on Linux.

I highly recommend using the _solarized_ Pygments color scheme, at least as long as there is no color scheme using the HoGent style colors. The package and installation instructions can be found in [this repository][solarized].

The compilation flag `-shell-escape` needs to be added to your LaTeX compiler. For **TeXstudio** go to _Options > Configure TeXstudio >  Commands_ and add it to the parameters for each compiler listed:
![TeXstudio](https://raw.githubusercontent.com/pvdk/hogent-latex-thesis/master/texstudio.png?raw=true)

## Contributing
Suggestions, feature requests, [issues](https://github.com/pvdk/hogent-latex-thesis/issues) and [pull requests](https://github.com/pvdk/hogent-latex-thesis/pulls) are always welcome.

## Todos
 - Support for multiple supervisors
 - Since Montserrat supports both serif and sans-serif, perhaps add serif?
 - Support for changing the various text fields on the title page
 - Add a 'draft' and 'final' mode
 - Support multiple document types, like thesis, project and abstract
 - Implement an 'abstract' page
 - Add a copyright/copyleft page

## Licensing
This template is released under the [MIT license][mitlicense].
The fonts that are used are licensed under the [SIL Open Font License][ofllicense].
A copy of the original license text for each font can be found in their respective folder under the fonts/ directory.

[www]: <https://github.com/pvdk/hogent-latex-thesis>
[latex]: <http://www.latex-project.org/>
[hogenttin]: <https://github.com/HoGentTIN/bachproef-latex-sjabloon>
[tudelft]: <https://www.tudelft.nl/en/tu-delft-corporate-design/downloads/>
[minted]: <https://ctan.org/pkg/minted/>
[pygments]: <http://pygments.org/>
[solarized]: <https://github.com/shkumagai/pygments-style-solarized/>
[montserrat]: <https://fonts.google.com/specimen/Montserrat>
[inconsolata]: <https://fonts.google.com/specimen/Inconsolata>
[firamath]: <https://github.com/firamath/firamath>
[ibmguide]: <https://www.ibm.com/support/knowledgecenter/en/SSAT72/com.ibm.help.empinstall_installing.doc/Installation/T_InstallingTeXLiveOnWindows.html>
[mactex]: <https://www.tug.org/mactex/>
[mitlicense]: <https://opensource.org/licenses/MIT/>
[ofllicense]: <https://opensource.org/licenses/OFL-1.1/>
[thesistex]: <https://github.com/pvdk/hogent-latex-thesis/tree/master/thesis.tex>
