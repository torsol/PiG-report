# Prosjektoppgave-Latex

## Requirements

* [Sublime Text 3](https://www.sublimetext.com/3)
* [ST Package Control](https://packagecontrol.io/installation)
* [ST LaTexTools](https://github.com/SublimeText/LaTeXTools#requirements-and-setup) is installed with Package Control
* [SyntaxFold](https://packagecontrol.io/packages/SyntaxFold#command-examples) is installed with Package Control
* [BufferScroll](https://github.com/titoBouzout/BufferScroll) Must be manually cloned to Packages folder
* For BibTex management, create user and install [Mendeley](https://mendeley.com/)

Insert this setting into Preferences > Package Settings > SyntaxFold > Settings - User:
`
{
    "scope": "text.tex.latex",
    "startMarker":"\\\\begin{info}",
    "endMarker":"\\\\end{info}"
}
`

### For Windows
* [MikTex](https://miktex.org)
* [Sumatra](https://www.sumatrapdfreader.org/download-free-pdf-viewer.html)
* After that you just need to build LaTeX document in SublimeText with CTRL+B
* Add Sumatra to PATH with e.g. `setx PATH %PATH%;C:\Program Files\SumatraPDF`
* Then you need to do some trickery with Sumatra. It is explained further [here](http://latextools.readthedocs.io/en/latest/install/)


### For Mac
* [MacTex](https://www.tug.org/mactex/)
* [Skim](http://skim-app.sourceforge.net)
* `sudo tlmgr install latexmk`
* In Skim: go to Preferences->Sync and set ‘preset’ to SublimeText.
* After that you just need to build LaTeX document in SublimeText with CMD+B



## Report writing guidelines
http://frigg.ivt.ntnu.no/ross/div/report.pdf

## Example report
http://frigg.ivt.ntnu.no/ross/div/thesis-0817.pdf

## Styling
* [Harvard-style referencing](https://www.ntnu.no/viko/harvard-eksempler)
* [English-style writing](http://www.ntnu.edu/english-matters/ntnu-english-style-guide)

## General info from NTNU
https://innsida.ntnu.no/masteroppgave

