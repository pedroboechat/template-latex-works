# A LaTeX template for academic works

## Table of contents

- [Introduction](#introduction)
- [Usage with Overleaf](#usage)
- [Overview](#overview)
- [Included packages](#packages)
- [Configuration](#config)

<h2 id="introduction"> Introduction </h2>

This template was made for allowing to easily create a new, ready-to-go LaTeX project for academic works. It ships with the most commonly used packages and is fully commented and documented. Also, it is modular in a way that you can easily add or remove any features from it.

<h2 id="usage"> Usage with Overleaf </h2>

[Overleaf](https://www.overleaf.com/) is a easy to use, online, collaborative LaTeX editor. To add this template to Overleaf:

1) Download the latest .zip file from the [releases section](https://github.com/pedroboechat/template-latex-works/releases) of this repository;
2) Follow this simple guide on [uploading a project](https://www.overleaf.com/learn/how-to/Uploading_a_project) to Overleaf.

<h2 id="overview"> Overview </h2>

The template contains a `main.tex` file, which is the main file of the project and contains package imports and the document creation.

The `./bibliography` folder is where to put .bib files for BibLaTeX and already has an empty `bibliography.bib` file.

The `./images` folder is where to put any image files you want to add to the project. It is used as graphicx's graphicspath, to avoid needing to add the full path to the image file (e.g. `./images/file.png` → `file.png`). There is, by default, a `minerva.png` file, containing [UFRJ](https://ufrj.br/)'s logo.

The `./sections` folder is where to put the .tex files containing the sections of your project, to be later included to `main.tex` with the `\subfile` command. Following a `##_sectionname.tex` naming pattern, it already contains a `00_title.tex` file, which is the template's title page, and a  sample `01_introduction.tex` file.

<h2 id="packages"> Included packages </h2>

- [abstract](https://ctan.org/pkg/abstract)

  ​	Gives control over the typesetting of the abstract environment.

- [amsmath](https://ctan.org/pkg/amsmath)

  ​	American Mathematical Society extensions for LaTeX. Contains math related utilities.

- [amssymb](https://ctan.org/pkg/amsmath)

  ​	Defines macros for mathematical symbols ([more info](http://milde.users.sourceforge.net/LUCR/Math/mathpackages/amssymb-symbols.pdf)).

- [appendix](https://ctan.org/pkg/appendix)

  ​	Allows extra control of appendices.

- [babel](https://ctan.org/pkg/babel)

  ​	Manages culturally-determined typographical rules for a wide range of languages.

- [biblatex](https://ctan.org/pkg/biblatex)

  ​	Bibliography system for adding citations and references.

- [caption](https://www.ctan.org/pkg/caption)

  ​	Allows extra control of captions.

- [csquotes](https://www.ctan.org/pkg/csquotes)

  ​	Provides advanced facilities for inline and display quotations.

- [enumerate](https://www.ctan.org/pkg/enumerate)

  ​	Gives the enumerate environment an optional argument which determines the style in which the counter is printed.

- [fancyhrd]()

  ​	Extensive facilities, both for constructing headers and footers, and for controlling their use.

- [float](https://www.ctan.org/pkg/float)

  ​	Improves the interface for defining floating objects such as figures and tables.

- [fontenc](https://ctan.org/pkg/fontenc)

  ​	Fixes encoding at the compiled PDF and allows to correctly copy glyphed text characters from it.

- [geometry](https://ctan.org/pkg/geometry)

  ​	Allows to customize page layout, implementing auto-centering and auto-balancing mechanisms.

- [graphicx](https://ctan.org/pkg/graphicx)

  ​	Improves the graphics package.

- [hyperref](https://ctan.org/pkg/hyperref)

  ​	Used to produce hypertext links in the document.

- [indentfirst](https://ctan.org/pkg/indentfirst)

  ​	Indents first paragraph after section header.

- [inputenc](https://ctan.org/pkg/inputenc)

  ​	Used to handle different input encodings in LaTeX files.

- [listings](https://ctan.org/pkg/listings)

  ​	Typeset source code listings.

- [minted](https://ctan.org/pkg/minted)

  ​	Highlights source code.

- [multicol](https://www.ctan.org/pkg/multicol)

  ​	Allows to typesets text in multiple columns.

- [mwe](https://www.ctan.org/pkg/mwe)

  ​	Helps to creates a minimal working example, such as minipages.

- [subfiles](https://www.ctan.org/pkg/subfiles)

  ​	Handles multi-file projects and improves importing of files.

- [tabularx](https://ctan.org/pkg/tabularx)

  ​	Allows to create tabulars with adjustable-width columns.

- [titling](https://www.ctan.org/pkg/titling)

  ​	Control over the typesetting of titling commands.

<h2 id="config"> Configuration </h2>

- Title page (`00_title.tex`)
  - At the file `00_title.tex` you can find the code for the title page.
  - At [line 5](https://github.com/pedroboechat/template-latex-works/blob/main/sections/00_title.tex#L5), there is the name of the subject (and it's subject code). In case you don't have or don't want it on the title page, you can remove lines 7 and 8 and uncomment line 11, which adds enough vertical spacing to keep the position for all other elements.
  - At [line 22](https://github.com/pedroboechat/template-latex-works/blob/main/sections/00_title.tex#L22), there is the inclusion of the institution logo. The template is using `minerva.png` image file inside `./images` folder.
  - At [line 30](https://github.com/pedroboechat/template-latex-works/blob/main/sections/00_title.tex#L30), there is the list of authors and their student registries and emails.
  - At [lines 43 to 45](https://github.com/pedroboechat/template-latex-works/blob/main/sections/00_title.tex#L43-L45), there is the abstract element. By default it is commented.
  - At [lines 51 and 52](https://github.com/pedroboechat/template-latex-works/blob/main/sections/00_title.tex#L51-L52), there is the information of place, date and semester.
- Main file (`main.tex`)
  - At the file `main.tex` you can find the main code of the project. All the packages imported in it are documented above in the [included packages](#packages) section of this README file. Some of then allow for additional configuration and are explained bellow.
  - At [line 2](https://github.com/pedroboechat/template-latex-works/blob/main/main.tex#L2), there is the definition of the project's document class as `article`.
  - At [line 5](https://github.com/pedroboechat/template-latex-works/blob/main/main.tex#L5), there is the definition of the paper type and margin.
  - At [line 18](https://github.com/pedroboechat/template-latex-works/blob/main/main.tex#L18), there is the definition of the project title, that will be used in the title page and can be retrieved anywhere in the project with the `\thetitle` command.
  - At [line 24](https://github.com/pedroboechat/template-latex-works/blob/main/main.tex#L24), there is the definition of language for `babel` package.
  - At [line 27](https://github.com/pedroboechat/template-latex-works/blob/main/main.tex#L27), there is the definition of `biblatex`'s bibliography and citation configuration.
  - At [lines 35 to 43](https://github.com/pedroboechat/template-latex-works/blob/main/main.tex#L35-L43), there is the PDF metadata definition with `hyperref` package.
  - At [line 47](https://github.com/pedroboechat/template-latex-works/blob/main/main.tex#L47), there is the definition of `\graphicspath` folder, which will be used as a "base path" for including graphics.
  - At [lines 56 to 60](https://github.com/pedroboechat/template-latex-works/blob/main/main.tex#L56-L60), there is the definition of `tabularx` column alignments for the `X` column type.
  - At [lines 67 to 72](https://github.com/pedroboechat/template-latex-works/blob/main/main.tex#L67-L72), there is the definition of the elements implemented with `fancyhdr` package. You can edit the pages header (`head`) and footer (`foot`) elements placed at the left (`l`), center (`c`) and right (`r`). By default, the left header element (`lhead`) has the project title and the central footer element (`cfoot`) has the page number.
  - At [lines 90 and 91](https://github.com/pedroboechat/template-latex-works/blob/main/main.tex#L90-L91), there is the overwriting of abstract's element font sizes.
  - At [lines 103 and 104](https://github.com/pedroboechat/template-latex-works/blob/main/main.tex#L103-L104), there is the definition of `csquotes` styling and the outer quote auto-formatting character shortcut.
  - At [line 111](https://github.com/pedroboechat/template-latex-works/blob/main/main.tex#L111), there is the import of the title page from `00_title.tex` file.
  - At [line 114](https://github.com/pedroboechat/template-latex-works/blob/main/main.tex#L114), there is creation of the table of contents by calling the `\tableofcontents` command.
  - At [line 117](https://github.com/pedroboechat/template-latex-works/blob/main/main.tex#L117), there is creation of the list of tables by calling the `\listoftables` command, along with commands to add it to the table of contents.
  - At [line 120](https://github.com/pedroboechat/template-latex-works/blob/main/main.tex#L120), there is creation of the list of figures by calling the `\listoffigures` command, along with commands to add it to the table of contents.
  - Between [lines 122 and 126](https://github.com/pedroboechat/template-latex-works/blob/main/main.tex#L122-L126) comments, there is a place reserved for importing subfiles (e.g. `01_introduction.tex` sample section file).
  - At [line 131](https://github.com/pedroboechat/template-latex-works/blob/main/main.tex#L131), there is creation of the bibliography by calling the `\printbibliography` command, with a parameter to add it to the table of contents.
  - At [line 139](https://github.com/pedroboechat/template-latex-works/blob/main/main.tex#L139), there is a sample import of an appendix file.