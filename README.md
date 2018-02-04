# Master thesis template for writing with Sublime Text

## Requirements

* [Sublime Text 3](https://www.sublimetext.com/3)
* [ST Package Control](https://packagecontrol.io/installation)
* [ST LaTexTools](https://github.com/SublimeText/LaTeXTools#requirements-and-setup) Install with Package Control
* [SyntaxFold](https://packagecontrol.io/packages/SyntaxFold#command-examples) Install with Package Control
* [BufferScroll](https://github.com/titoBouzout/BufferScroll) Manually clone to Packages folder
* [Mendeley](https://mendeley.com/) For BibTex management, create user and install desktop program + browser add-on

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

## Key-bindings 
### Windows/Mac
* Compile the PDF: `ctrl+B` / `cmd+B`
* Manually Showing Completions (for image files, references etc): `ctrl+space`
* Forward search: `ctrl+l, j` / `cmd+l, j`
	* i.e. jump to the point in the PDF file where the cursor position is. 
	* Let go of `ctrl/cmd` when pressing `j`
* Backward search: `ctrl+shift+mouseclick` / `cmd+shift+mouseclick`
	* i.e. jump to the point in the source code where click happens

## Report writing guidelines
http://frigg.ivt.ntnu.no/ross/div/report.pdf

## Example report
http://frigg.ivt.ntnu.no/ross/div/thesis-0817.pdf

## Styling
* [Harvard-style referencing](https://www.ntnu.no/viko/harvard-eksempler)
* [English-style writing](http://www.ntnu.edu/english-matters/ntnu-english-style-guide)

## General info from NTNU
https://innsida.ntnu.no/masteroppgave

