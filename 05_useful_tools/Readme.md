## Useful tools 

This part of the repository contains curated tools that can be helpful to prepare different types of files in formats that can be uploaded into cBioportal. 

## What you will find here 

You will find each tool in a separate folder. Within this folder there will be a readme with detailed instructions on how to use the tool, an overview of how the folder is structured and an example study that you can use as a template to test the tool. Those folders that have a number preceding their folder name have been tested by us (Example: 01_Data_processor). We will keep updating these as we test the tools, so visit back for updates on these tools.
## Overview of tools 

This is a summary of all the tools you will find in this part of the repository.

| Tool Name                                                                                          | Description                                                                             | Advantages                                                                                          | Disadvantages                                                                                                           | FH Repository Link                                                                                     |
|----------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------|
| [Data-processor](https://github.com/MJKorte/Data-processor)                                     | Formats clinical data tables in multi-tab Excel files to cBioportal format             | - Useful for varied clinical data fields.<br>- Supports multi-tab Excel files.<br>- Easy terminal execution | - Does not seem to work to generate clinical data files.<br>- Requires adherence to specific clinical data variable names from [cBioPortal Clinical Data Dictionary] | [Data_processor](https://github.com/FredHutch/tg-cbioportal-data/tree/main/05_useful_tools/01_Data_processor) |
| [cbpManager](https://github.com/arsenij-ust/cbpManager)                                         | An R-based Shiny App that allows users to create and upload cBioPortal-formatted studies. | - A relatively easy to run R based (Shiny) App.<br>- Allows you to create clinical data files, timeline related files, and mutation files.<br>- Allows users to run the validation of their formatted study folders | - Currently only helps to create clinical and mutation data related files.<br>- If using the app to create the files then can only update one patient at a time | [cbpManager](https://github.com/FredHutch/tg-cbioportal-data/tree/main/05_useful_tools/02_cbpManager)       |
| [CaisisTools (a FH tool)](https://github.com/FredHutch/CaisisTools)                             | Takes clinical data in the form of an excel workbook and converts to cBioportal format | - Helpful for processing clinical data.<br>- Can be used for data from RedCap                      | - Data either must be obtained from Caisis or should be in the same format                                           | [CaisisTools](https://github.com/FredHutch/tg-cbioportal-data/tree/main/05_useful_tools/CaisisTools)        |
| [Varan 2.0](https://github.com/bioinformatics-policlinicogemelli/Varan-Pub/tree/v2.1.1)        | Takes genomic data and existing study folder to process and upload into cBioportal.    | - Useful for validating an existing cBioportal study folder.<br>- Can concatenate from multi-sample vcf files.<br>- Can be used to do filtering of genomic files | - Has several local dependencies (vcf2maf, VEP, and samtools).<br>- Folder preparations restricted to CNV, SNV, SV, and clinical data | [Varan](https://github.com/FredHutch/tg-cbioportal-data/tree/main/05_useful_tools/Varan-Pub)                |
| [cBioPortal-BS-Lab](https://github.com/BS-Laboratory/cBioPortal)                               | Helpful scripts to take data from RedCap to convert to clinical data files             | - Good for demonstrating how to take data stored in RedCap and format                              | - Mostly would be useful for clinical data files                                                                        | [cBioPortal-BS-Lab](https://github.com/FredHutch/tg-cbioportal-data/tree/main/05_useful_tools/cBioPortal-BS-Lab) |
| [cBioPortal_Importer](https://github.com/oicr-gsi/cBioPortal_Importer)                        | Python script to prepare data for uploads into cBioportal. Mostly genomics data.      | - Helpful scripts to transform specific data types into cBioportal format                           | - Accepts very specific output files.<br>- Requires threshold setting for copy number data, etc.                      | [cBioPortal_Importer](https://github.com/FredHutch/tg-cbioportal-data/tree/main/05_useful_tools/cBioPortal_Importer) |
| [cbpConverter](https://github.com/WeiChenPan/cbpConverter)                                     | R Shiny App to convert Excel sheets into cBioportal format                             | - Seems like a simple Shiny app to convert clinical data into cBioportal format                     | - Looks untested but might have helpful scripts.<br>- Again only clinical data                                      | [cbpConverter](https://github.com/FredHutch/tg-cbioportal-data/tree/main/05_useful_tools/cbpConverter)      |
| [gdc-et-pipeline](https://github.com/cBioPortal/gdc-et-pipeline)                               | Converts data from the GDC repository to cBioportal format                             | - If data is available on GDC, this might be useful                                               | - Written in Java.<br>- File formats have to be in the GDC format.<br>- Folder preparations restricted to CNV, SNV, Expression, and clinical data | [gdc-et-pipeline](https://github.com/FredHutch/tg-cbioportal-data/tree/main/05_useful_tools/gdc-et-pipeline) |
| [kf-cbioportal-etl](https://github.com/kids-first/kf-cbioportal-etl)                          | Specific to this study: CAVATICA and Data Warehouse                                   | - Helpful scripts that can be leveraged.                                                           | - These scripts might be specific to the format of files found in this study.                                        | [kf-cbioportal-etl](https://github.com/FredHutch/tg-cbioportal-data/tree/main/05_useful_tools/kf-cbioportal-etl) |
| [mutational-signature-converter](https://github.com/dippindots/mutational-signature-converter) | Very specifically converts the mutational signature data into cBioportal format        | - Helps to convert mutational signature data into cBioPortal format                                | - Has not been updated in a few years.<br>- Simple python script                                                    | [mutational-signature-converter](https://github.com/FredHutch/tg-cbioportal-data/tree/main/05_useful_tools/mutational-signature-converter) |
| [shah-cbioportal-tools](https://github.com/shahcompbio/cbioportal-tools)                      | Specifically for formatting Copy Number Data expects a seg file and TITAN output      | - Could potentially be used for tools other than TITAN that generate a seg file                   | - Specific for TITAN outputs                                                                                          | [shah-cbioportal-tools](https://github.com/FredHutch/tg-cbioportal-data/tree/main/05_useful_tools/shah-cbioportal-tools) |
