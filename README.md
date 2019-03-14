# awesome-bioinformatics-formats
Curated list of bioinformatics formats and publications. Not every format here is "awesome" persay, but if you are
thinking about creating a new format this could be your first place to look at potential pre-existing formats. We also
include formats not specific to bioinformatics, but should be considered for bioinformatics applications.

Please feel free to [contribute](https://github.com/kmhernan/awesome-bioinformatics-formats/blob/master/CONTRIBUTING.md).

**Table of Contents**

- [Formats](#formats)
  - [General](#general)
  - [Dense Genomic Data](#dense-genomic-data)
  - [Genomic Intervals](#genomic-intervals)
  - [Genotype Data](#genotype-data)
  - [Unaligned Sequencing Data](#unaligned-sequencing-data)
  - [Aligned Sequencing Data](#aligned-sequencing-data)
  - [Miscellaneous](#miscellaneous)
- [Review Papers and Blogs](#review-papers-and-blogs)

----

## Formats

### General

Formats not specific to bioinformatics that should be considered.

* [HDF5](https://portal.hdfgroup.org/display/support) - HDF5 is a data model, library, and file format for storing and managing data. It supports an unlimited variety of datatypes, and is designed for flexible and efficient I/O and for high volume and complex data. HDF5 is portable and is extensible, allowing applications to evolve in their use of HDF5. The HDF5 Technology suite includes tools and applications for managing, manipulating, viewing, and analyzing data in the HDF5 format.
* [NetCDF](https://www.unidata.ucar.edu/software/netcdf/) - Network Common Data Form is a set of interfaces for array-oriented data access and a freely distributed collection of data access libraries for C, Fortran, C++, Java, and other languages.
* [SQLite](https://sqlite.org/index.html) - SQLite is a C-language library that implements a small, fast, self-contained, high-reliability, full-featured, SQL database engine.
* [tiledb](https://tiledb.io/) - TileDB manages massive dense and sparse multi-dimensional array data that frequently arise in important scientific applications.

### Dense Genomic Data

Formats associated with storing dense functional genomics data.

* [bigWig](https://genome.ucsc.edu/goldenPath/help/bigWig.html) - The bigWig format is useful for dense, continuous data and is a binary form of [wiggle](https://genome.ucsc.edu/goldenPath/help/wiggle.html).
* [Genomedata](https://academic.oup.com/bioinformatics/article/26/11/1458/203307) - a format for efficient storage of multiple tracks of numeric data anchored to a genome.
* [GenomicsDB](https://www.genomicsdb.org/) - GenomicsDB is an open sourced library and tools with a focus on optimizing sparse array storage specifically for genomic data.
* [wiggle](https://genome.ucsc.edu/goldenPath/help/wiggle.html) - ASCII format for dense, continuous data.

### Genomic Intervals

Formats associated with storing genomic intervals (e.g., contig, start, stop, strand).

* [BED](https://genome.ucsc.edu/FAQ/FAQformat.html#format1) - Browser Extensible Data format provides a flexible way to define the data lines that are displayed in an annotation track.
* [bedGraph](https://genome.ucsc.edu/goldenPath/help/bedgraph.html) - The bedGraph format allows display of continuous-valued data in track format.
* [bigBed](https://genome.ucsc.edu/goldenPath/help/bigBed.html) - Binary and indexed form of [BED](https://genome.ucsc.edu/FAQ/FAQformat.html#format1).
* [narrowPeak](https://genome.ucsc.edu/FAQ/FAQformat.html#format12) - This format is used to provide called peaks of signal enrichment based on pooled, normalized (interpreted) data. It is a BED6+4 format.
* [segmentation file](https://software.broadinstitute.org/software/igv/SEG) - A tab-delimited text file that lists loci and associated numeric values associated with copy number.
* [tabix](http://samtools.github.io/hts-specs/tabix.pdf) - An *index* file format for genomic intervals (can be used on bed, gtf, vcf, etc).

### Genomic Features

Formats for describing genomic features (e.g., gene models, etc.).

* [genePred](http://genome.ucsc.edu/FAQ/FAQformat#format9) - a table format commonly used for gene prediction tracks.
* [GFF](https://github.com/The-Sequence-Ontology/Specifications/blob/master/gff3.md) - The general feature format is a file format used for describing genes and other features of DNA, RNA and protein sequences.
* [GTF](http://mblab.wustl.edu/GTF22.html) - GTF stands for Gene transfer format. It borrows from [GFF](https://github.com/The-Sequence-Ontology/Specifications/blob/master/gff3.md), but has additional structure that warrants a separate definition and format name.

### Genotype Data

Formats associated with genotype data.

* [BCF](http://samtools.github.io/hts-specs/BCFv2_qref.pdf) - Binary and compressed [VCF](http://samtools.github.io/hts-specs/VCFv4.3.pdf) format.
* [GVF](https://github.com/The-Sequence-Ontology/Specifications/blob/master/gvf.md) - The Genome Variation Format (GVF) is a very simple file format for describing sequence_alteration features at nucleotide resolution relative to a reference genome.
* [VCF](http://samtools.github.io/hts-specs/VCFv4.3.pdf) - Variant Call Format.
* [oxford-gen](https://www.cog-genomics.org/plink2/formats#gen) - Native text genotype file format for Oxford statistical genetics tools, such as IMPUTE2 and SNPTEST.
* [plink-bed](https://www.cog-genomics.org/plink2/formats#bed) - PLINK binary biallelic genotype table.

### Unaligned Sequencing Data

Formats associated with storing unaligned sequencing data.

* [FASTA](https://en.wikipedia.org/wiki/FASTA_format) - ASCII format for storing nucleotide/amino acid sequences.
* [FASTQ](https://academic.oup.com/nar/article/38/6/1767/3112533) - Designed as a replacement for FASTA, combining the sequence and quality information in the same file.

### Aligned Sequencing Data

Formats associated with storing aligned sequencing data.

* [BAM](http://samtools.github.io/hts-specs/SAMv1.pdf) - Binary [SAM](http://samtools.github.io/hts-specs/SAMv1.pdf) format. _note: it is becoming more common to store unaligned reads in a BAM called a uBAM_
* [CRAM](http://samtools.github.io/hts-specs/CRAMv3.pdf) - Further lossless compression of [SAM](http://samtools.github.io/hts-specs/SAMv1.pdf) format.
* [MAF](https://genome.ucsc.edu/FAQ/FAQformat.html#format5) - The multiple alignment format stores a series of multiple alignments in a format that is easy to parse and relatively easy to read. 
* [SAM](http://samtools.github.io/hts-specs/SAMv1.pdf) - The Sequence Alignment/Map format.

### Miscellaneous 

Formats that currently don't have a good section to place them yet (but still very relevant).

* [BIOM](http://biom-format.org/) - The Biological Observation Matrix (BIOM) file format (canonically pronounced biome) is designed to be a general-use format for representing biological sample by observation contingency tables.

## Review Papers and Blogs

This section contains links to relevant review papers and blog posts about bioinformatics formats.

* [hts-specs](http://samtools.github.io/hts-specs/) - From the great Heng Li.

