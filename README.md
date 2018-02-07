# Master thesis template for writing with Sublime Text

## Requirements

* [Sublime Text 3](https://www.sublimetext.com/3)
* [ST Package Control](https://packagecontrol.io/installation)
* [ST LaTexTools](https://github.com/SublimeText/LaTeXTools#requirements-and-setup) Install with Package Control
* [SyntaxFold](https://packagecontrol.io/packages/SyntaxFold#command-examples) Install with Package Control
* [BufferScroll](https://github.com/titoBouzout/BufferScroll) Manually clone to Packages folder
* [Mendeley](https://mendeley.com/) For BibTex management, create user and install desktop program + browser add-on
* [Spell checking](https://github.com/titoBouzout/Dictionaries) Manual download

## Settings
### Insert this setting into Preferences > Package Settings > SyntaxFold > Settings - User:

	{
	    "scope": "text.tex.latex",
	    "startMarker":"\\\\begin{info}",
	    "endMarker":"\\\\end{info}"   
	}
	
This thesis template contains info-box environments. These can be hidden/folded in the source code with key-bidning `alt-0-0`

### Insert this into Preferences > Package Settings > Package Control > Settings - User:
`
"install_prereleases": ["LaTeXTools"],
`

LaTeXTools uses pre-releases to beta test new features and improve the stability of releases. This enables graphicx package support, that let's us preview images in the source code by hovering over the filenames.

## Installation

### For Windows
* [MikTex](https://miktex.org) LaTex for windows
* [Sumatra](https://www.sumatrapdfreader.org/download-free-pdf-viewer.html) PDF viewer for compiling LaTex to PDF
* Add Sumatra to PATH with e.g. `setx PATH %PATH%;C:\Program Files\SumatraPDF`
* Then you need to do some trickery with Sumatra. It is explained further [here](http://latextools.readthedocs.io/en/latest/install/)

### For Mac
* [MacTex](https://www.tug.org/mactex/) LaTex for Mac
* [Skim](http://skim-app.sourceforge.net) PDF viewer for compiling LaTex to PDF
* `sudo tlmgr install latexmk`
* In Skim: go to Preferences->Sync and set ‘preset’ to SublimeText.

## Usage
Open as a Sublime Project by opening the file `thesis.sublime-project`.

By default, the document is in *draft* mode, which means info boxes with tips to writing will appear. This also makes compilation faster as it simplifies the document by not including figures, hyperrefs etc.
**Turn draft mode off** by switching to _final_ within the documentclass at the very top of main.tex.

Add new chapters and sections in new files as you like, and import them in the main.tex file. 

Put all figures in the `Figures/` folder. Figures in this directory can be included from any tex-file in the project using file name only, e.g. `\includegraphics{logo_ntnu)`. You can then hover over the file name to get a preview of the image.

## Key-bindings 
### Here `C`denotes `ctrl` for windows / `cmd` for mac
| Description 			|	Key-binding 	| Tip  |
|----------------------	|---------------	|------|
| **Compile the PDF**	|	`C+b`			| Choose _PdfLaTex_ if prompted     |
| **New environment** 	|	`C+l, C+n`		| While holding `C`, press `l` then `n`|
| **Bold text**			|	`C+l, C+b`		|      |
| **Italic text**		|	`C+l, C+e`		|      |
| **Forward search**	|	`C+l, j`		| Let go of `C` before pressing `j`.	<br> Jumps to the point in the _PDF_ <br> file where the cursor position <br> is in the source code. |
| **Backward search** 	|	`C+shift+click`	| Jumps to the point in the <br> _tex-file_ corresponding <br> to the mouse click in the PDF|
| **Go to anything**	|	`C+r`			| For fast navigation within a file|
| **LaTex Completions**	|	`C+l, x`		| Let go of `C` before pressing `j`. <br> Gives suggestions within `\ref{}`, <br> `\cite{}` and `\figures{}`|
| **Other completions**	|	`C+space`		| For functions etc|
| **Fold info environments**|	`alt+0+0`	| Folds/hides all info environments <br> in the tex-file|
| **Unfold info environments**|`alt+shift+0+0`| Opens all info environments <br> in the tex-file |

## Report writing guidelines
http://frigg.ivt.ntnu.no/ross/div/report.pdf

## Example report
http://frigg.ivt.ntnu.no/ross/div/thesis-0817.pdf

## Styling
* [Harvard-style referencing](https://www.ntnu.no/viko/harvard-eksempler)
* [English-style writing](http://www.ntnu.edu/english-matters/ntnu-english-style-guide)

## General info from NTNU
https://innsida.ntnu.no/masteroppgave

