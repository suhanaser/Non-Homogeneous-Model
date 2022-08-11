# Non-Homogeneous-Model
A pipline to test for homogeneity in large datasets
### Installation
To run this script you need Python 3 and the following dependencies: Biopython, math, itertools, numpy, pandas, shutil, glob, random, and linecache. 
### Running the script
First you should define the clades in a text file as follows:
1. If you have n taxa that you want to group in k clades then your text file should include k lines that represents the different clades.
    Each line have the names of the taxa in that clade, separated by a coma.You can find an example in `clades.txt`
2. Run `Extract_clades_alignmet.py` as follow:
```
Extract_clades_alignments.py <alignment_file> <alignment_fromat> <clades_file> <clades_dir>
<alignment_file>    The full alignment with all taxa
<alignment_fromat>  The format of the alignment. possible formats: fasta, phylip, or nexus
<clades_file>       text file that where each line represents a clade. Taxa in each clade/line are separated by a coma. e.g.clades.txt
                    Note: make sure that the taxa names are the same as they appear in the alignment file.
<clades_dir>        Directory where you want to save all the clades' alignments
```
