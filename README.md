# Plant Genomics Tool Overview

A large number of tools is available for various tasks in plant genomics. This repository provides an overview about available (and recommended) tools in plant genomics. This is based on the experiences of the [Plant Biotechnology and Biotechnology](https://www.tu-braunschweig.de/en/ifp/pbb) research group at TU Braunschweig. If you are new to plant genomics, our ['Data Literacy in Plant Genomics'](https://doi.org/10.1515/jib-2023-0033) course might be of interest to you.




## Handling reads

ToolName | Comments | Reference
--- | --- | ---
guppy | ONT basecalling | [ONT](https://community.nanoporetech.com/docs/prepare/library_prep_protocols/Guppy-protocol/v/gpb_2003_v1_revax_14dec2018/guppy-software-overview)
[fastQC](https://github.com/s-andrews/FastQC) | quality control short reads | FastQC GitHub repository
[LongQC](https://github.com/yfukasawa/LongQC) | quality control long reads | [Fukasawa et al., 2020](https://doi.org/10.1534/g3.119.400864)
[Filtlong](https://github.com/rrwick/Filtlong) | trimming long reads | Filtlong GitHub repository
[Trimmomatic](http://www.usadellab.org/cms/?page=trimmomatic) | trimming short reads | [Bolger et al., 2014](https://doi.org/10.1093%2Fbioinformatics%2Fbtu170)


## Genome sequence assembly

ToolName | Comments | Reference
--- | --- | ---
[HiCanu](https://github.com/marbl/canu) | long read assembler (resource intensive) | [Nurk et al., 2020](https://doi.org/10.1101%2Fgr.263566.120)
[NextDenovo2](https://github.com/Nextomics/NextDenovo) | long read assembler | GitHub repository
[Shasta](https://github.com/paoloshasta/shasta) | long read assembler (fast) | [Shafin et al., 2020](https://doi.org/10.1038/s41587-020-0503-6)
[Flye](https://github.com/fenderglass/Flye) | long read assembler (high memory requirements) | [Kolmogorov et al., 2019](https://doi.org/10.1038/s41587-019-0072-8)
[miniasm](https://github.com/lh3/miniasm) | long read assembler | [Li, 2018](https://doi.org/10.1093/bioinformatics/btw152)


## Repeat masking & annotation

ToolName | Comments | Reference
--- | --- | ---
[RepeatMasker](https://github.com/rmhubley/RepeatMasker) | masking/annotating repeats; Repbase needed | Smit, AFA, Hubley, R & Green, P. RepeatMasker Open-4.0. 2013-2015 <http://www.repeatmasker.org>.
[EDTA](https://github.com/oushujun/EDTA) | repeat annotation | [Ou et al., 2019](https://doi.org/10.1186/s13059-019-1905-y)
panEDTA | pangenome repeat annotation | [Ou et al., 2022](https://doi.org/10.1101/2022.10.09.511471)


## Read mapping

ToolName | Comments | Reference
--- | --- | ---
[STAR](https://github.com/alexdobin/STAR) | RNA-seq read mapping | [Dobin et al., 2013](https://doi.org/10.1093%2Fbioinformatics%2Fbts635)
[HISAT2](http://daehwankimlab.github.io/hisat2/) | RNA-seq read mapping | [Kim et al., 2019](https://doi.org/10.1038/s41587-019-0201-4)
[minimap2](https://github.com/lh3/minimap2) | long read mapping | [Li, 2018](https://doi.org/10.1093/bioinformatics/bty191)


## Gene prediction

ToolName | Comments | Reference
--- | --- | ---
[BRAKER3](https://github.com/Gaius-Augustus/BRAKER) | protein coding gene prediction | [Gabriel et al., 2023](https://doi.org/10.1101/2023.06.10.544449)
[Augustus](https://github.com/Gaius-Augustus/Augustus) | protein coding gene prediction | [Stanke et al., 2006](https://doi.org/10.1093/nar/gkl200)
[GeMoMa](http://www.jstacs.de/index.php/GeMoMa) | protein coding gene prediction | [Keilwagen et al., 2019](https://doi.org/10.1007/978-1-4939-9173-0_9)
[TSEBRA]() |  | 
tRNA-scanSE2 |  | 

## Comparative genomics

ToolName | Comments | Reference
--- | --- | ---
MCscan | | 
TBtools-II | | 
TOGA | | 


## Functional annotation

KIPEs, MYB_annotator, bHLH_annotator, Mercator, InterProScan5, BLAST2GO, KeggMapper





## Further Reading
There are also specific collection of tools for particular purposes: 

[Long-Read-Tools](https://long-read-tools.org/)


If you have questions about plant genomics that were not answered by any of these resources, please feel free to get in touch with the Plant Biotechnology and Biotechnology research group at TU Braunschweig.
