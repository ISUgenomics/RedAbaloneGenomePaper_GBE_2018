# RedAbaloneGenomePaper_GBE_2018

## An Annotated Genome for Haliotis rufescens (Red Abalone) and Resequenced Green, Pink, Pinto, Black and White Abalone Species
Rick Masonbrink1, Catherine Purcell2, Sara Boles3
Andrew Whitehead3, John Hyde4, Arun Seetharam1, Andrew Severin1*

1 Genome Informatics Facility, Iowa State University, 206 Science I, Ames, IA 50011, USA
2 Ocean Associates, Inc. under contract to NOAA Fisheries, Southwest Fisheries Science Center, 8901 La Jolla Shores Drive, La Jolla, CA 92037, USA
3 Department of Environmental Toxicology, University of California Davis, CA 95616, USA
4 NOAA Fisheries, Southwest Fisheries Science Center, 8901 La Jolla Shores Drive, La Jolla, CA 92037, USA

*Author for Correspondence: E-mail: severin@iastate.edu
Data deposition
Raw data along with the genome assembly are submitted to NCBI under the bioproject ID PRJNA434455

**Keywords:**
Red abalone; genome assembly; aquaculture; Haliotis; Haliotis rufescens

#### Abstract

Abalone are one of the few marine taxa where aquaculture production dominates the global market as a result of increasing demand and declining natural stocks from overexploitation and disease. To better understand abalone biology, aid in conservation efforts for endangered abalone species, and gain insight into sustainable aquaculture, we created a draft genome of the red abalone (Haliotis rufescens). The approach to this genome draft included initial assembly using raw Illumina and Pacific Biosciences (PacBio) sequencing data with MaSuRCA, before scaffolding using sequencing data generated from Chicago library preparations with HiRise2. This assembly approach resulted in 8,371 scaffolds with a total length of 1.498 gb; the N50 of the assembly was 1.895 mb, and the longest scaffold was 13.2 Mb.  Gene models were predicted, using Maker2, from RNA-Seq data and all related ESTs and proteins from NCBI; this resulted in 57,785 genes with an average length of 8,255 bp. In addition, SNPs were called on Illumina short-sequencing reads from five other eastern Pacific abalone species: the green (H. fulgens), pink (H. corrugata), pinto (H. kamtschatkana), black (H. cracherodii), and white (H. sorenseni) abalone. Phylogenetic relationships largely follow patterns detected by previous studies based on 1,784,991 high quality SNPs from the 96,084,900 SNPs identified from the six species. Among the six abalone species examined, the endangered white abalone appears to harbor the lowest levels of heterozygosity. This draft genome assembly and the sequencing data provide a foundation for genome-enabled aquaculture improvement for red abalone, and for genome-guided conservation efforts for the other five species and, in particular, for the endangered white and black abalone.


#### Supplemental data files.

##### GenomeScope

Estimates of heterozygosity and repetitiveness were measured from the raw paired-end Illumina data using GenomeScope.  Below are the jellyfish kmer files for k = 21 that is the input for Genomescope.

* [Black abalone](Genomescope/black_reads_K21.histo)
* [Green abalone](Genomescope/green_reads_K21.histo)
* [Pink abalone](Genomescope/pink_reads_K21.histo)
* [Pinto abalone](Genomescope/pinto_reads_K21.histo)
* [Red abalone](Genomescope/red_reads_K21.histo)
* [White abalone](Genomescope/white_reads_K21.histo)


##### MAKER2
Four rounds of maker were run as we added different types of data to improve the gene models. Below are the Maker control files with all the settings to replicate our analysis.

* [Round1: ESTs and data from NCBI and Transcripts generated from red abalone RNA-Seq data](MAKER2/Round1_maker_opts.ctl)
* [Round2: SNAP HMM round 1](MAKER2/Round2_maker_opts.ctl)
* [Round3: SNAP HMM round 2](MAKER2/Round3_maker_opts.ctl)
* [Round4: with genemark and busco/augustus training](MAKER2/Round4 _maker_opts.ctl)

##### Phylogenetic tree
The File below can be used to visualize the phylogenetic tree generated in the paper using [FigTree v1.4.3](http://tree.bio.ed.ac.uk/software/figtree/)

[tree input file](phylogeneticTree/Figure3.tree)
