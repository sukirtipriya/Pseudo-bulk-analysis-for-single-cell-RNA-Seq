# Pseudo-bulk-analysis-for-single-cell-RNA-Seq

To compare gene expression across individuals, one may first estimate cell type-specific gene expression per individual by adding up the RNA-seq counts of all the cells of the same cell type. This is often known as pseudo-bulk RNA-seq data.

the current best practice is using a pseudobulk approach, which involves the following steps:

    Subsetting to the cells for the cell type(s) of interest to perform the DE analysis.
    Extracting the raw counts after QC filtering to be used for the DE analysis
    Aggregating the counts and metadata to the sample level.
    Performing the DE analysis (Need at least two biological replicates per condition to perform the analysis, but more replicates are recommended).
