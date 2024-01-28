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
[RepeatMasker](https://github.com/rmhubley/RepeatMasker) | masking/annotating repeats; Repbase needed | [Smit, et al., 2015](http://www.repeatmasker.org)
[EDTA](https://github.com/oushujun/EDTA) | repeat annotation | [Ou et al., 2019](https://doi.org/10.1186/s13059-019-1905-y)
panEDTA | pangenome repeat annotation | [Ou et al., 2022](https://doi.org/10.1101/2022.10.09.511471)


## Read mapping

ToolName | Comments | Reference
--- | --- | ---
[STAR](https://github.com/alexdobin/STAR) | RNA-seq read mapping | [Dobin et al., 2013](https://doi.org/10.1093%2Fbioinformatics%2Fbts635)
[HISAT2](http://daehwankimlab.github.io/hisat2/) | RNA-seq read mapping | [Kim et al., 2019](https://doi.org/10.1038/s41587-019-0201-4)
[minimap2](https://github.com/lh3/minimap2) | long read mapping | [Li, 2018](https://doi.org/10.1093/bioinformatics/bty191)


## Variant calling and annotation

ToolName | Comments | Reference
--- | --- | ---
[BWA MEM](https://github.com/lh3/bwa) | short read mapping | [Li, 2013](https://doi.org/10.48550/arXiv.1303.3997)
[GATK](https://gatk.broadinstitute.org/hc/en-us) | short read variant calling | [Van der Auwera GA & O'Connor BD., 2020](https://www.oreilly.com/library/view/genomics-in-the/9781491975183/)
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
[BUSCO](https://busco.ezlab.org/) | assembly/annotation completeness check | [Manni et al., 2021](https://doi.org/10.1002/cpz1.323)

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
[BLAST](https://blast.ncbi.nlm.nih.gov/Blast.cgi) | sequence comparison | [Altschul et al., 1990](https://doi.org/10.1016/s0022-2836(05)80360-2)
[DIAMOND](https://github.com/bbuchfink/diamond) | | [Buchfink et al., 2015](https://doi.org/10.1038/nmeth.3176)
[HMMER](http://hmmer.org/) | sequence comparison | [Finn et al., 2011](https://doi.org/10.1093%2Fnar%2Fgkr367)
[KAAS](https://www.genome.jp/kegg/kaas/) | assigning KEGG IDs | [Moriya et al., 2007](https://doi.org/10.1093%2Fnar%2Fgkm321)
[ENTAP](https://github.com/harta55/EnTAP) | - | [Hart et al., 2019](https://doi.org/10.1111/1755-0998.13106)
[eggNOG-mapper](https://github.com/eggnogdb/eggnog-mapper) | assigning eggNOG IDs | [Cantalapiedra et al., 2021](https://doi.org/10.1093/molbev/msab293)


## Coexpression analyses

ToolName | Comments | Reference
--- | --- | ---
[fastq-dump](https://github.com/ncbi/sra-tools/wiki/HowTo:-fasterq-dump) | FASTQ downloads | NCBI
[kallisto](https://github.com/pachterlab/kallisto) | gene expression quantification | [Bray et al., 2016](https://doi.org/10.1038/nbt.3519)
[WGCNA](https://cran.r-project.org/web/packages/WGCNA/index.html) | coexpression analysis | [Langfelder & Horvath, 2008](https://doi.org/10.1186/1471-2105-9-559)
[GENIE3](https://bioconductor.org/packages/release/bioc/html/GENIE3.html) | coexpression analysis | [Huynh-Thu et al., 2010](https://doi.org/10.1371/journal.pone.0012776)
[dynGENIE3](https://github.com/vahuynh/dynGENIE3) | coexpression analysis | [Huynh-Thu & Geurts, 2018](https://doi.org/10.1038/s41598-018-21715-0)


## Phylogenetic analyses

ToolName | Comments | Reference
--- | --- | ---
[MAFFT](https://mafft.cbrc.jp/alignment/software/) | multiple sequence alignment | [Katoh & Standley, 2013](https://doi.org/10.1093/molbev/mst010)
[MUSCLE](https://www.drive5.com/muscle/) | multiple sequence alignment | [Edgar, 2022](https://doi.org/10.1038/s41467-022-34630-w)
[IQ-TREE2](https://doi.org/10.1093/molbev/msaa015) | phylogenetic tree construction | [Minh et al., 2020](https://doi.org/10.1093/molbev/msaa131)
[FastTree](http://www.phylo.org/index.php/tools/fasttree_xsede.html) | phylogenetic tree construction | [Price et al., 2010](https://doi.org/10.1371%2Fjournal.pone.0009490)
[RAxML-NG](https://github.com/amkozlov/raxml-ng) | phylogenetic tree construction | [Kozlov et al., 2019](https://doi.org/10.1093/bioinformatics/btz305)
[SHOOT](https://www.shoot.bio/) | phylogenetic placement of sequence | [Emms & Kelly, 2022](https://doi.org/10.1186/s13059-022-02652-8)
[iTOL](https://itol.embl.de/) | phylogenetic tree visualization | [Letunic & Bork, 2021](https://doi.org/10.1093/nar/gkab301)
[JustOrthologs](https://github.com/ridgelab/JustOrthologs) | ortholog identification | [Miller et al., 2019](https://doi.org/10.1093/bioinformatics/bty669)
[SwiftOrtho](https://github.com/Rinoahu/SwiftOrtho) | ortholog identification | [Hu & Friedberg, 2019](https://doi.org/10.1093/gigascience/giz118)


## Helpful databases

ToolName | Comments | Reference
--- | --- | ---
[jbrowse]() | | 
[gbrowse]() | | 
[TAIR]() | | 
[Phytozome]() | | 
[JGI Plant Gene Atlas]() | | 
[SRA]() | | 
[GEO]() | | 
[OrthoDB]() | | 
genome hubs generally


## Further Reading
There are also specific collection of tools for particular purposes: 

[Long-Read-Tools](https://long-read-tools.org/)


If you have questions about plant genomics that were not answered by any of these resources, please feel free to get in touch with the Plant Biotechnology and Biotechnology research group at TU Braunschweig.
