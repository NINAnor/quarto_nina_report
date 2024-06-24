# NINA-report template using Quarto
This is a Quarto template for creating NINA-reports. This is not the same as https://github.com/NINAnor/NINA-ebook-template, which is intended to create a more general web-page.

Typically, you would use this template in Rstudio to create a NINA-report from an R-script. It replaces the Rmarkdown NINA-report template in the NinaR package (https://github.com/NINAnor/NinaR). A key benefit of using Quarto instead of Rmarkdown is that you don't need to change any code, such as cross-references in order to switch between formats. This means you can easily switch between the output formats pdf, html and docx using the same template.

The template is under sporadic development. If you have suggestions or problems, please create an issue here in Github. Specific problems can be related to Jens Åström by email, but I can't promise to answer promptly or constructively. The PDF version is fully operational and conforms to the new NINA-report Word template, the one that was (or will soon be?) updated in 2024. This is the version where you fill in the metadata in a form when you first open the template. The html version has some basic NINA-styling but will probably be amended in the future. The Word version is unstyled. It doesn't make much sense to create a NINA-report Word styling and there are no plans develop the Word version further.

This template requires a working installation of XelaTeX. This is installed at least on NINA's Rstudio servers. To use, run this in the terminal window on a machine with a Quarto installation (From within NINA, typically https://rstudio.nina.no). 

```sh
quarto use template NINAnor/quarto_nina_report
```

This creates a subfolder in the folder you are standing in (in the terminal), with a file called 'quarto_ninatemplate.qmd'. Create a copy of this file with a name that reflects the name of the report. Render this through the "render" button in Rstudio. It may be a good idea to keep the original qmd-document as well as a another minimal example, which you use to test out new features with shorter rendering times.

Please see https://quarto.org/docs/get-started/hello/rstudio.html for a general tutorial on how to use this. Specific tips are found in the template itself.


