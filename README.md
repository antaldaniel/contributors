## Welcome 👋

🙋‍♀️ Creating an ecosystem of open data and open knowledge sharing in R, hugo, and open science repositories.

🌈 Contribution guidelines - you must abide by the [Contributor Covenant](https://www.contributor-covenant.org/version/2/1/code_of_conduct/) Code of Conduct.

**Major releases**
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10259347.svg)](https://doi.org/10.5281/zenodo.10259347)

The source files in this repository may contain small edits that are not yet reflected in the [Digital Music Observatory](https://zenodo.org/communities/music_observatory?q=&l=list&p=1&s=10&sort=newest) community repository on Zenodo.

- `0.2.1`: The tidying of the KULT microdata documentation is added as an annex (2023-12-13.)

## Ignored files in .gitignore
We place a list of folders and files that are ignored for synchronization from the user’s client computer to Github and beyond.  These are usually passwords, login credentials, project management or log files used by your IDE or other work environment.  We by default, excluded all Posit/RStudio standards, and usually all Jupiter Notebook standards, and a few Windows/Mac specific files.
We also ignore a standard folder called `not_included`,  which serves as the place of your personal scrapbook, sandbox, that you do not want to share with anybody.

## Data folders

We have two data folders, which may have numerous subfolders.

`data-raw`:  Raw, unprocessed data, as received, downloaded, collected. Please try to ingest data as well-documented as possible.  If the ingestion is not done by our reproducible tools that log the download, copying, and bibliographic references, you are requested to create a standard bibliographic reference for any data that you place here. You can use your favorite citation management tool or join our shared, open-source, Zotero account, but eventually, the data asset must be added to the bib/data-raw.bib files as a standard, BibLatex data citation. We use the DataCite standard, which almost fully corresponds to DublinCore.

`data`: This folder contains the processed data or our outputs.  Any data here must adhere to the tidy data principle and be documented by DataCite standards.  We are developing a tool, dataset, which will do this automatically in WP4.  We can investigate a Python connector for this if there is a need for that.
Bibliographic reference folders.

## Referencing and attribution

`bib`: Contains all bibliography: used citations, data used, visualisation used, datasets created, visualizations created, public text document outputs created.


## Visualisation folders

We save visualisations in folders corresponding to the file format. This is the best way to ensure that pandoc or any compiles has the necessary plugins to work with the visualizations. Every visualization that is intended to made pubic gets a bibliographic citation and a globally unique DOI identifier. 

`png`: contains visualisations in Portable Network Graphics format (our preferred format.)

`jpg`: Contains visualization in Joint Photographic Experts Group format.

`webp`: Contains visualisations in WebP is an open image file format developed by Google intended as a replacement for JPEG, PNG, and GIF file formats.  We prefer this for content intended for web use (presentations, blogposts), because it works much faster and better with browsers than PNG or JPG.

[…] You can use other formats if necessary.


## Program code folders
`R`: contains any script in the R language.

`Py`: contains script in the Python language [if there is any, create the folder at first time use].

`CPP`: contains script in the C++ language [if there is any, create the folder at first time use].

## Text markup folders
`tex`: Tex document markup language templates.
`css` : CSS style templates [if there is any, create the folder at first time use].

## Final text outputs 

The final text outputs are in the `_book` folder.  They are weaved together by pandoc, knitr and bookdown if they are made of several source files, hence the name book. If they are created from a single file, they are not technically a book but they are here in HTML, EPUB, PDF, or docx or pptx formats. 

## Source texts

The source texts are stored in Rmd, md, or tex files in the main folder.  We prefer Rmd, because Posit can integrate well R, Python, C++ code, and via pandoc and knitr various Latex and Word compilers.  But you can use any flavor of .md or .tex. 

 Rmd is technically a plan .md with a special YAML heading for machine use and optional R, Python, or C++ code placeholders. If you decide to use other .md editors, we will create an empty template that contains the non-visible YAML heading for machine processing.
