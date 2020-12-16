# cfMeDIP-seq-analysis-pipeline
Post-processing pipeline for next-generation circulating methylome data generated by cfMeDIP-seq

## Dependencies

The only up-front dependency is Anaconda.

Key Anaconda package dependencies:

- pyyaml
- mamba (conda-forge)
- snakemake (bioconda)
- picard (bioconda)
- samtools (bioconda)
- bwa (bioconda)
- R packages: dplyr, data.table
- R Bioconductor packages: MEDIPS, bsgenome.hsapiens.ucsc.hg19

## Snakemake profiles

For a guide on how to create a Snakemake profile for your cluster setup, see https://www.sichong.site/2020/02/25/snakemake-and-slurm-how-to-manage-workflow-with-resource-constraint-on-hpc/

# Setup Notes

- `GenomeInfoDb` and `GenomeInfoDbData` were not properly installed by conda. Installed these after the fact with BiocManager.
