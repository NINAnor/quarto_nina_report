# NINA-report template using Quarto

<!-- badges: start -->
[![DOI](https://zenodo.org/badge/734397304.svg)](https://doi.org/10.5281/zenodo.16946726)
<!-- badges: end -->

This is a Quarto template for creating NINA-reports. This is not the same as https://github.com/NINAnor/NINA-ebook-template, which is intended to create a more general web-page.

This template is only tested to work on Linux-machines. You are welcome to adopt it to work on windows machines and submit a pull-request. Typically, you would use this template in Rstudio to create a NINA-report from an R-script. It replaces the Rmarkdown NINA-report template in the NinaR package (https://github.com/NINAnor/NinaR). A key benefit of using Quarto instead of Rmarkdown is that you don't need to change any code, such as cross-references in order to switch between formats. This means you can easily switch between the output formats pdf, html and docx using the same template.

The template is under sporadic development. If you have suggestions or problems, please create an issue here in Github. Specific problems can be related to Jens Åström by email, but I can't promise to answer promptly. The PDF version is fully operational and conforms to the current (< 2026) NINA-report Word template. The html version has some basic NINA-styling but will probably be amended in the future. The Word version is unstyled. It doesn't make much sense to create a NINA-report Word styling and there are no plans develop the Word version further.

This template requires a working installation of XelaTeX. This is installed at least on NINA's Rstudio servers. To use, run this in the terminal window on a machine with a Quarto installation (From within NINA, typically https://rstudio.nina.no). 

```sh
quarto use template NINAnor/quarto_nina_report
```

This creates a subfolder in the folder you are standing in (in the terminal), with a file called 'quarto_ninatemplate.qmd'. Create a copy of this file with a name that reflects the name of the report. Render this through the `Render` button in Rstudio. It may be a good idea to keep the original qmd-document as well as a another minimal example, which you use to test out new features with shorter rendering times.

The functionality of this template is affected by the interplay between versions of Tex, Pandoc and Quarto. To resolve possible problems on rstudio.nina.no, and to use this template on other machines, you can work with standalone versions of Tex and Quarto. Install TinyTeX with "tinytex::install_tinytex()". Download the latest quarto version at https://quarto.org/docs/download/. Extract this in your home folder in e.g. ~/quarto.

To make sure R finds the right versions, add this to your ~/.Renviron file (create it if it doesn't exist)

`
QUARTO_PATH="~/quarto/quarto-1.8.26/bin/quarto"
`
`
QUARTO_TINYTEX="~/.TinyTex"
`

To make sure quarto is discoverable by the system, add this last in ~/.bashrc:

`
PATH="$USER/quarto/quarto-1.8.26/bin:$PATH"
`

This is tested to work on rstudio-geo.nina.no and a standalone Linux machine.


Please see https://quarto.org/docs/get-started/hello/rstudio.html for a general tutorial on how to use this. Specific tips are found in the template itself.

## Changelog
### V2.0
Embeds custom fonts and babel-norsk. This makes it work on a linux machine without prior Texlive installation and no superuser rights.

### V1.x
Changes not tracked



