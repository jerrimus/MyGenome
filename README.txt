Genes for Good Genotypes Download Version 1.2
=============================================

Thank you for participating in Genes for Good! 

Contents of this README
-----------------------

I.    What Is In Your Download
II.   What File Formats Are Present
III.  How To Read Your Genotypes
IV.   Data Integrity and Risk Disclaimer
V.    Recommended Text-Based Tools For Viewing Genotypes
VI.   Graphical/Interactive Tool Options
VII.  Genotype Version History
VIII. Additional Information and Further Reading


I. What Is In Your Download
---------------------------

You have just downloaded a ZIP archive containing the following 9 files:

1. GFG_filtered_unphased_genotypes.vcf.gz
2. GFG_filtered_unphased_genotypes.vcf.gz.tbi
3. GFG_filtered_unphased_genotypes_23andMe.txt
4. GFG_filtered_unphased_genotypes_vcf.txt
5. GFG_filtered_imputed_genotypes_noY_noMT.vcf.gz
6. GFG_filtered_imputed_genotypes_noY_noMT.vcf.gz.tbi
7. GFG_filtered_imputed_genotypes_noY_noMT_23andMe.txt
8. GFG_filtered_imputed_genotypes_noY_noMT_vcf.txt
9. README.txt

Files 1-4 contain different formats of the list of about 500,000 positions in your DNA (your genotypes) directly measured by software at Genes for Good. The genotypes are quality-controlled but we have made no attempt to interpret your genotypes. For example, we have not attempted to figure out which genotypes may carry disease risk.

Files 5-8 contain your imputed genotypes. That means we estimated genotypes at an additional 7 million positions by comparing your directly measured genotypes to a set of 2,500 people whose genotypes have already been determined, and filling in the best guesses for your DNA bases we did not directly measure. Because these files contain imputed and not directly measured genotypes, there is a greater chance of errors. Also, some text editors may not be able to open these files because of their larger size.

File 9 is this README file.


II. What File Formats Are Present
---------------------------------

Files 4 and 8 are text files (.txt) in uncompressed Variant Call Format (VCF) v4.1. These files will open in a text program, but you may not be able to understand what everything says. Please see below for more details to help you understand how the information is displayed.

Files 1 and 5 are zipped VCF files (.vcf.gz). This is a standardized text file format used in bioinformatics and you may not be able to read it on your computer.

Files 2 and 6 are Tabix indexes (.vcf.gz.tbi) that accompany the zipped VCF files and are not readable by humans, but allow some bioinformatics tools to analyze the compressed VCF file faster.

Files 3 and 7 are text files (.txt) with your data in a more easily  readable 23andMe format.


III. How To Read Your Genotypes
-------------------------------

If you are viewing a VCF file using a text editor, then a typical genotype may look like this:

1	798959	rs11240777	G	A	.	PASS	.	GT	0/0

The first column indicates the number of the chromosome, 1, where this genetic marker is found. 

The second column contains "798959", which is the position or number of bases from this marker to the end of the chromosome. 

The third column contains "rs1124077", which is the name of this marker. We attempted to use names assigned by the National Center for Biotechnology Information and these begin with "rs". Other markers have generic names that we generated.

The fourth column contains "G", which is the first of two possible alleles that participants can have at this marker. This G refers to the genetic base guanine.

The fifth column contains "A", which is the second possible allele that a participant can have at this marker. This A refers to the genetic base adenine.

The sixth column is required as part of the VCF format but we do not use it. In these files, it contains a dot.

The seventh column contains the word "PASS", indicating that this marker passed our internal quality control protocols.

The eighth column is also required as part of the VCF format but we do not use it. In these files, it contains a dot.

Finally, the ninth column contains "0/0", which is the genotype for this participant at this marker. Specifically, "0/0" means that this participant has two copies -- one on each copy of chromosome 1 -- of the reference allele, which column four indicates is G in this case. A "0/1" genotype would mean that this participant has a copy of both the reference allele, G, and the alternate allele, A. "1/1" would mean that this participant has two copies of the alternate allele, A.

In the files with the imputed genotypes, a pipe "|" instead of a slash "/" in the genotype indicates that we have attempted to phase this genotype, which means we attempt to determine which allele in each pair belongs on which chromosome. We estimate the alleles on the left of the pipe to all be on the same physical chromosome, and the alleles on the right of the pipe on the other copy of the chromosome.

The genotype would look like the following in the 23andMe format:

rs11240777	1	798959	GG

This indicates that this person has two copies of the G allele at rs11240777, which is located on chromosome 1 at position 798959.


IV. Data Integrity and Risk Disclaimer
--------------------------------------

Generally speaking, we expect a small percentage of your genotypes to be wrong. We do not know where those errors are and cannot correct them.

Although we do everything we can to ensure high quality standards in sample handling and data generation, unexpected things can happen and we are not able to detect or correct all types of errors.

Genes for Good is a research study. The technology and protocols we use are suitable for genetic research, not for clinical genetic testing such as you would receive at a hospital or doctor’s office.

Clinical genetic testing is held to higher standards. Laboratories which handle these samples are certified by governmental regulations called CLIA.

In the United States, methods used to diagnose disease or recommend treatment must be approved by the FDA. The genotypes we have generated have not been reviewed by the FDA.

Our genotype lab is NOT FDA-approved or CLIA-certified! This approval and certification is not necessary for a research study.

For more info see: https://www.cms.gov/clia

Other risks associated with attempting to understand your genetic data include discovering that a family member was adopted or their biological parents or siblings may not be who they believed them to be.

There are also risks associated with storing your genetic information on a personal computer or other medium of electronic storage. Take care to protect these data.


V. Recommended Text-Based Tools For Viewing Genotypes
-----------------------------------------------------

Many word processing programs will fail to open the text files in your download because the files are too big and word processors are optimized to work with smaller, richly formatted documents.

To maximize your ability to view the very large text files in your download, consider using any of the following free text editors:

Windows:
* glogg - http://glogg.bonnefon.org/download.html
* Notepad++ - https://notepad-plus-plus.org/
* Vim/gVim - http://www.vim.org/download.php

Mac:
* TextWrangler http://www.barebones.com/products/textwrangler/
* Vim/gVim - http://www.vim.org/download.php

Unix/Linux:
* glogg - http://glogg.bonnefon.org/download.html
* Vim/gVim - http://www.vim.org/download.php

Whichever text editor you use, loading such large text files requires lots of memory (RAM), so consider also closing any other programs running when you try to load and view your data.


VI. Graphical/Interactive Tool Options
--------------------------------------

IMPORTANT NOTE

None of the options listed below are explicitly recommended by Genes For Good. This is merely a list of available software packages and websites for viewing and working with raw genetic data curated to include options with wider accessibility and ease of use. None of these options or the developers or companies associated with them are associated with Genes For Good in any way and their inclusion in this section does not constitute an endorsement of their software.

Use third-party software for viewing your raw genetic data at your own risk. It is your responsibility to research any software that you install, purchase, or otherwise load your data into.

* Integrative Genomics Viewer
  Type: Software Download OR Website (Java Applet)
  OS:   Windows, Mac, Linux
  URL:  https://www.broadinstitute.org/igv/viewing_vcf_files
  Free, requires registering an account with Broad Institute website

* Savant Genome Browser
  Type: Software Download
  OS:   Windows, Mac, Linux
  URL:  http://genomesavant.com/p/savant/download
  Free, open source, may require automatic reformatting of files

* Diploid
  Type: Software Download
  OS:   Mac
  URL:  http://www.diploid.com/differ
  Free, requires registering email with website

If you have used and enjoyed other websites or software to view and work with your raw genetic data then please contact Genes For Good to recommend the solution that worked best for you. We may want to include it in this list for all participants!


VII. Genotype Version History
-----------------------------

The processing pipeline we use for generating participant genotype data is an active project. Periodically a new version of genotype data will be released. Typically new versions may have slightly more accurate data from improved or optimized methods, or may present new data extracted from the same samples that was not present in earlier versions.

You can determine with certainty which version you have by checking the version number on the first line of this file. At any given time only the most current version will be available for participants to download.

Change Log:

* Version 1.2 - July 2016
  More RS numbers - We now have RS numbers for 97% of the variants in the unimputed files and 99.7% in the imputed.
  A new imputation reference panel for X-nonPAR that has about 2,000 fewer variants.

* Version 1.1 - June 2016
  More RS numbers, indels added to 23andMe format files, other minor changes to improve speed and memory usage in the generation pipeline

* Version 1.0 - September 2015
  Initial release of results including ancestry pie chart, chromosome painting, PCA plot, and downloadable genotypes


VIII. Additional Information and Further Reading
------------------------------------------------

For a brief introduction on human genetics that may be useful in attempting to understand these files, please see: https://www.genome.gov/25520880

The Variant Call Format (VCF) was developed by the 1000 Genomes Consortium and is maintained by the Global Alliance for Genomics and Health Data. The format specification is available at: http://samtools.github.io/hts-specs/VCFv4.1.pdf

Basing health decisions on genetic data is risky. This article in The Atlantic provides some further insight into such risks: http://www.theatlantic.com/science/archive/2015/12/why-human-genetics-research-is-full-of-costly-mistakes/420693/

This README file is also available online at the address: https://genesforgood.sph.umich.edu/readme/readme1.2.txt

Thank you again for your participation!
