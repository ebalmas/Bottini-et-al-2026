# Bottini-et-al.-2026
Code repository for the bioinformatic analysis of Bottini et al 2026

# Download the supporting "scratch folders" from the Zenodo repository:
Use wget or download directly on [Zenodo](https://doi.org/10.5281/zenodo.21471692).
Place the code in a folder together with the "scratch folder" and rename it "scratch"; then you can repeat the analysis within our Docker.

# Download the Docker image to allow reproducibility

The Docker images used for these scripts are:

```hedgelab/rstudio-hedgelab:iPS2seq_new_cellranger7```

```hedgelab/rstudio-hedgelab:iPS2seq_new_cellranger9```


These Images can run CellRanger (either CellRanger 7 or CellRanger 9) on the bash server and the R code on the RStudio server.

Code example for RStudio server:

```docker run -d -itv /path/to/shared/folder:/scratch --privileged=true -p 8080:8787 --name container_name hedgelab/rstudio-hedgelab:iPS2seq_new_cellranger7```


```docker exec -idt container_name rstudio-server start```

Then go to the browser http://localhost:8080/

Below is the link to the raw data; the codes are in a folder named with the bioStudies code.

Bulk RNA-sequencing comparison of GERALT circuit architectures and OPTi-OX during MYOD1-driven skeletal muscle differentiation of WTC11 hiPSCs[E-MTAB-17408](https://www.ebi.ac.uk/biostudies/arrayexpress/studies/E-MTAB-17408)

Bulk RNA-sequencing analysis of TGFβ withdrawal and receptor inhibition in parental and DRACH-mutant NANOG-overexpressing WTC11 hiPSCs[E-MTAB-17410](https://www.ebi.ac.uk/biostudies/arrayexpress/studies/E-MTAB-17410)

Single-cell transcriptomic profiling of NANOG-overexpressing and parental WTC11 hiPSCs during prolonged TGFβ withdrawal [E-MTAB-17411](https://www.ebi.ac.uk/biostudies/arrayexpress/studies/E-MTAB-17411)

pip seq-Single-Cell Transcriptomic Comparison of Primary, Wild-Type, and MYOD1-Overexpressing Cells During Skeletal Muscle Differentiation [E-MTAB-17414](https://www.ebi.ac.uk/biostudies/arrayexpress/studies/E-MTAB-17414)
