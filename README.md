# quarto_nina_report
A quarto template for NINA-reports. The basic functionality works, but there might be some quirks to fix.

You can switch between the output formats pdf, html and docx using the same template. A key benefit of using quarto is that you don't need to change any code, such as cross-references in order to switch between formats.

So far, only the PDF version is fully operational, which requires a working installatin of XelaTeX (works at least on NINA's Rstudio servers). The html version has some basic NINA-styling. The Word version is unstyled, and it doesn't make obvious sense to create a NINA-report word styling.  

To use, run this in the terminal window on a machine with a Quarto installation (For NINA, typically https://rstudio.nina.no). This will create a subfolder in the folder you are standing in (in the terminal). 

```sh
quarto use template NINAnor/quarto_nina_report
```

You will find additional instructions in the template 'quarto_ninatemplate.qmd'. Rename this to suit your needs. It may be a good idea to keep another minimal qmd-document as well, to test out new features with shorter rendering times.

