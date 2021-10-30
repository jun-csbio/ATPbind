# ATPbind: 
An Accurate Protein-ATP binding residue prediction method.

## Pre-requisite:
    - Python, Java, Perl
    - SANN software (https://github.com/newtonjoo/sann)
    - NCBI nr90 database (ftp://ftp.ncbi.nlm.nih.gov/blast/db/FASTA/)
    - Linux system (suggested CentOS 7)

## Installation:

*Download this repository at https://github.com/jun-csbio/ATPbind.git first. Then, uncompress it and run the following command lines on Linux System.
~~~
  $ java -jar FileUnion.jar ./standalone-package-fragments/ ./ATPbind.zip
  $ unzip ATPbind.zip
  $ cd ./ATPbind
  $ cd ./software
  $ chmod -R 777 ./*
~~~

*The file of "./jar/Config.properties" should be set as follows:
~~~
# FIXED_CONFIGS
VISITER_COUNT=../Visiter_count.txt
WEB_SERVER_NAME=ATPbind
LOG_FOLDER_DIR=../Log
BLASTPGP_SSITE_OUTPUT_PARSER_DIR=../software/junh_BlastpgpSSITEOutputPARSER
ATP_SSITE_LIBDIR=../library
SSITE_EXE_PATH=../software/junh_TMSITEatp_Templ_Searcher/ssite
ATP_TMSITE_LIBDIR=../library
TMSITE_TEMPL_SEARCHER_DIR=../software/junh_TMSITEatp_Templ_Searcher
BLASTPGP_EXE_PATH=../software/blast-2.2.26/blastpgp
BLAST_BIN_DIR=../software/blast-2.2.26
PSIPRED321_FOLDER_DIR=../software/psipred321
ATPbind8SEQ_MODEL0_PATH=../MODEL/ATPseqMol0
ATPbind8SEQ_MODEL1_PATH=../MODEL/ATPseqMol1
ATPbind8SEQ_MODEL2_PATH=../MODEL/ATPseqMol2
ATPbind8SEQ_MODEL3_PATH=../MODEL/ATPseqMol3
ATPbind8SEQ_MODEL4_PATH=../MODEL/ATPseqMol4
ATPbind8SEQ_MODEL5_PATH=../MODEL/ATPseqMol5
ATPbind8SEQ_MODEL6_PATH=../MODEL/ATPseqMol6
ATPbind8SEQ_MODEL7_PATH=../MODEL/ATPseqMol7
ATPbind8SEQ_MODEL8_PATH=../MODEL/ATPseqMol8
ATPbind8SEQ_MODEL9_PATH=../MODEL/ATPseqMol9
ATPbind8SEQ_REPORT_THRESHOLD=0.42
ATPbind8STRUCT_MODEL0_PATH=../MODEL/ATPbindMol0
ATPbind8STRUCT_MODEL1_PATH=../MODEL/ATPbindMol1
ATPbind8STRUCT_MODEL2_PATH=../MODEL/ATPbindMol2
ATPbind8STRUCT_MODEL3_PATH=../MODEL/ATPbindMol3
ATPbind8STRUCT_MODEL4_PATH=../MODEL/ATPbindMol4
ATPbind8STRUCT_MODEL5_PATH=../MODEL/ATPbindMol5
ATPbind8STRUCT_MODEL6_PATH=../MODEL/ATPbindMol6
ATPbind8STRUCT_MODEL7_PATH=../MODEL/ATPbindMol7
ATPbind8STRUCT_MODEL8_PATH=../MODEL/ATPbindMol8
ATPbind8STRUCT_MODEL9_PATH=../MODEL/ATPbindMol9
ATPbind8STRUCT_REPORT_THRESHOLD=0.38
ITASSER_STRUCT_FOLDER=../ITASSER_STRUCT
IND_TEST_SEQ_2_NAME_ON_ATPSEQ=../IND_TEST_RES/seq2id.fa
IND_TEST_RES_FOLDER=../IND_TEST_RES/


# SHOULD BE CHANGED
BLASTPGP_DB_PATH=xxx/nr
SANN_RUNNER_PATH=yyy/sann.sh
~~~

Note that, "xxx" should be the absolute path of the downloaed NCBI nr90 database. "yyy" should be the absolute path of the installed SANN software.

## Run the following commands to obtain the tips. 
~~~
  $ cd ./ATPbind/jar
  $ java -jar ATPbind.jar
~~~

## Update History:

- First release 2021-10-31

## Notes:
	Web server: https://zhanggroup.org/ATPbind/
	Contact : (Jun Hu) junh_cs@126.com
	
## References

[1] Jun Hu, Yang Li, Yang Zhang, and Dong-Jun Yu. ATPbind: accurate protein-ATP binding site prediction by combining sequence-profiling and structure-based comparisons [J]. Journal of Chemical Information and Modeling, 2018, 58(2): 501-510.
