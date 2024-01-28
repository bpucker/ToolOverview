# Plant Genomics Tool Overview

Many tools are available for various tasks in plant genomics. Finding the right tool for a certain purpose can be a challenge. This repository provides an overview about available (and recommended) tools in plant genomics. This is based on the experiences of the [Plant Biotechnology and Biotechnology](https://www.tu-braunschweig.de/en/ifp/pbb) research group at TU Braunschweig. If you are new to plant genomics, our ['Data Literacy in Plant Genomics'](https://doi.org/10.1515/jib-2023-0033) course might be of interest to you.




## Handling reads

ToolName | Comments | Reference
--- | --- | ---
guppy | ONT basecalling | [ONT](https://community.nanoporetech.com/docs/prepare/library_prep_protocols/Guppy-protocol/v/gpb_2003_v1_revax_14dec2018/guppy-software-overview)
[fastQC](https://github.com/s-andrews/FastQC) | quality control short reads | FastQC GitHub repository
[LongQC](https://github.com/yfukasawa/LongQC) | quality control long reads | [Fukasawa et al., 2020](https://doi.org/10.1534/g3.119.400864)
[Filtlong](https://github.com/rrwick/Filtlong) | trimming long reads | Filtlong GitHub repository
[Trimmomatic](http://www.usadellab.org/cms/?page=trimmomatic) | trimming short reads | [Bolger et al., 2014](https://doi.org/10.1093%2Fbioinformatics%2Fbtu170)


## Genome size estimation
ToolName | Comments | Reference
--- | --- | ---
[MGSE](https://github.com/bpucker/MGSE) | mapping-based | [Pucker, 2019](https://doi.org/10.1101/607390)
[GenomeScope2](https://github.com/schatzlab/genomescope) | k-mer-based | [Ranallo-Benavidez, 2020](https://doi.org/10.1038/s41467-020-14998-3)
[findGSE](https://github.com/schneebergerlab/findGSE) | k-mer-based | [Sun et al., 2017](https://doi.org/10.1093/bioinformatics/btx637)
[gnodes](http://arthropods.eugenes.org/EvidentialGene/other/gnodes/) | mapping-based | [Gilbert, 2022](https://doi.org/10.1101/2022.05.13.491861)


## Genome sequence assembly

ToolName | Comments | Reference
--- | --- | ---
[HiCanu](https://github.com/marbl/canu) | long read assembler (resource intensive) | [Nurk et al., 2020](https://doi.org/10.1101%2Fgr.263566.120)
[NextDenovo2](https://github.com/Nextomics/NextDenovo) | long read assembler | GitHub repository
[Shasta](https://github.com/paoloshasta/shasta) | long read assembler (fast) | [Shafin et al., 2020](https://doi.org/10.1038/s41587-020-0503-6)
[Flye](https://github.com/fenderglass/Flye) | long read assembler (high memory requirements) | [Kolmogorov et al., 2019](https://doi.org/10.1038/s41587-019-0072-8)
[miniasm](https://github.com/lh3/miniasm) | long read assembler | [Li, 2018](https://doi.org/10.1093/bioinformatics/btw152)
[QUAST](https://github.com/ablab/quast) | assembly statistics calculation | [Gurevich et al., 2013](https://doi.org/10.1093%2Fbioinformatics%2Fbtt086)


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


## Variant calling and annotation
[BWA MEM](https://github.com/lh3/bwa) | short read mapping | [Li, 2013](https://doi.org/10.48550/arXiv.1303.3997)
[GATK](https://gatk.broadinstitute.org/hc/en-us) | short read variant calling | Van der Auwera GA & O'Connor BD. (2020). Genomics in the Cloud: Using Docker, GATK, and WDL in Terra (1st Edition). O'Reilly Media.
[SVIM2](https://github.com/eldariont/svim) | long read variant calling | [Heller & Vingron, 2019](https://doi.org/10.1093/bioinformatics/btz041)
[Sniffles2](https://github.com/fritzsedlazeck/Sniffles) | long read variant calling | [Smolka et al., 2024](https://doi.org/10.1038/s41587-023-02024-y)
[SnpEff](http://pcingola.github.io/SnpEff/) | variant impact prediction | [Cingolani et al., 2012](https://doi.org/10.4161%2Ffly.19695)
[NAVIP](https://github.com/bpucker/NAVIP) | variant impact prediction | [Baasner et al., 2019](https://doi.org/10.1101/596718)


## Gene prediction

ToolName | Comments | Reference
--- | --- | ---
[BRAKER3](https://github.com/Gaius-Augustus/BRAKER) | protein coding gene prediction | [Gabriel et al., 2023](https://doi.org/10.1101/2023.06.10.544449)
[Augustus](https://github.com/Gaius-Augustus/Augustus) | protein coding gene prediction | [Stanke et al., 2006](https://doi.org/10.1093/nar/gkl200)
[GeMoMa](http://www.jstacs.de/index.php/GeMoMa) | protein coding gene prediction | [Keilwagen et al., 2019](https://doi.org/10.1007/978-1-4939-9173-0_9)
[TSEBRA](https://github.com/Gaius-Augustus/TSEBRA) | merge annotations | [Gabriel et al., 2021](https://doi.org/10.1186/s12859-021-04482-0)
[tRNAscan-SE](http://lowelab.ucsc.edu/tRNAscan-SE/) | tRNAs, rRNAs | [Chan et al., 2021](https://doi.org/10.1093/nar/gkab688)
BUSCO

## Comparative genomics

ToolName | Comments | Reference
--- | --- | ---
[MCscan](https://github.com/tanghaibao/jcvi/wiki/MCscan-(Python-version)) | synteny analysis | [Wang et al., 2012](https://doi.org/10.1093%2Fnar%2Fgkr1293)
[TBtools-II](https://github.com/CJ-Chen/TBtools-II) | comparative genomics | [Chen et al,. 2023](https://doi.org/10.1016/j.molp.2023.09.010)
[TOGA](https://genome.senckenberg.de/) | synteny analysis | [Kirilenko et al., 2023](http://dx.doi.org/10.1126/science.abn3107)


## Functional annotation

ToolName | Comments | Reference
--- | --- | ---
[InterProScan5](https://github.com/ebi-pf-team/interproscan) | universal functional annotation | [Jones et al., 2014](https://doi.org/10.1093/bioinformatics/btu031)
[KIPEs](https://github.com/bpucker/KIPEs) | biosynthesis pathway annotation | [Rempel et al., 2023](https://doi.org/10.1371/journal.pone.0294342)
[MYB_annotator](https://github.com/bpucker/MYB_annotator) | R2R3-MYB annotation | [Pucker, 2022](https://doi.org/10.1186/s12864-022-08452-5)
[bHLH_annotator](https://github.com/bpucker/bHLH_annotator) | bHLH annotation | [Thoben & Pucker, 2023](https://doi.org/10.1186/s12864-023-09877-2)
[Mercator](https://www.plabipd.de/mercator_main.html) | universal functional annotation | [Lohse et al., 2014](https://doi.org/10.1111/pce.12231)
[BLAST2GO](https://www.blast2go.com/) | universal functional annotation | [Conesa et al., 2005](https://doi.org/10.1093/bioinformatics/bti610)
[KEGG Mapper](https://www.genome.jp/kegg/mapper/) | KEGG ID assignment | [Kanehisa & Sato, 2020](https://doi.org/10.1002/pro.3711)

BLAST
DIAMOND
HMMER
KAAS (Kegg)


ENTAP
eggNOG-mapper



jbrowse
gbrowse
TAIR
genome hubs generally

## Coexpression analyses
fastq-dump
kallisto
WGCNA
GENIE3
dynGENIE3


## Phylogenetic analyses
MAFFT
MUSCLE
IQ-TREE2
FastTree
RAxML-NG
SHOOT
iTOL
JustOrthologs
SwiftOrtho


## Helpful databases
Phytozome
JGI Plant Gene Atlas
SRA/ENA/DDBJ
GEO
OrthoDB



## Further Reading
There are also specific collection of tools for particular purposes: 

[Long-Read-Tools](https://long-read-tools.org/)


If you have questions about plant genomics that were not answered by any of these resources, please feel free to get in touch with the Plant Biotechnology and Biotechnology research group at TU Braunschweig.
