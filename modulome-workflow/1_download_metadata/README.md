# Download RNAseq metadata

This folder contains scripts to download and format all RNA-seq metadata for an organism from NCBI Sequence Read Archive. To simplify the process, we have created a docker container with all pre-requisite software.

## Example usage

The following code finds all RNA-seq data for *Bacillus subtilis* and saves the data to the file `Bacillus_subtilis.tsv`. Note that the species name **must** be enclosed in quotes.

```bash
docker run --rm -it avsastry/get-all-rnaseq:latest "Bacillus subtilis" > Bacillus_subtilis.tsv
```
