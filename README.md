# Curve fitting and IC50 calculation using R

## Files for download.

- "MiMB2024-ploidy_SampleData.csv" is a datasheet containing raw data of dose-response cell proliferation assay for two inhibitors in isogenic ploidy series of HAP1 cells.
  - Doxorubicin: a topoisomerase II inhibitor. No ploidy-associated efficacy change was observed.
  - GSK-923295: a CENP-E inhibitor. Hyperploidy-selective efficacy increase was observed.
- "MiMB2024-ploidy_Script.Rmd" is a R markdown to calculate IC50s from dose-response curve of growth proliferation provided in "MiMB2024-ploidy_SampleData.csv".

## How to use

1. Download "MiMB2024-ploidy_Script.Rmd" and "MiMB2024-ploidy_SampleData.csv" to your working directory.
2. Open the Rmd file in Rstudio.
3. Run all chancks from the top down.
   - Updating packages would be required.
5. New folder named "output_MiMB2024-ploidy" is automatically made and following files are outputted:
   - df_nlr.csv is a datasheet containing parameters of curve fitting and IC50 values for all conditions.
   - MiMB2024-ploidy_plot_CGA_IC50.png shows plots of dose-response curve and IC50s.
   - NLR_MiMB2024-ploidy (folder) contains 48 plots of experimental data and fitted curve for all conditions.

## Remarks

- See sessionInfo.txt for the versions of R, Rstudio, and packages used in the Rmd file.

## Article info

1. K. Yoshizawa et al., Tetraploidy-linked sensitization to CENP-E inhibition in human cells, Molecular Oncology 17 (6) (2023) 1148–1166. doi:10.1002/1878-0261.13379
2. K. Yoshizawa and R. Uehara, Comparative pharmacological analysis of mitotic inhibitors using isogenic ploidy series of HAP1 cells, submitted to Methods in Molecular Biology
