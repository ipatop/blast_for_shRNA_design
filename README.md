# blast_for_shRNA_design

This python script implements qblast from Biopython on shRNA sequences.

To run it you will need python2 and biopython (https://github.com/biopython/biopython).

This program blasts online from a file with the Template. name and sequence separeted by a tab: 

CaMKI:TwXj1O_f	ctagcagtCCGATGGCAAGCTGCTCGGTAtagttatattcaagcataTACCGAGCAGCTTGCCATCGGgcg

Taking the first sequence of uppercase letterrs (using the indices(8:29) of the sequence) and online qblast taking the 20 best results (for case of equal transcripts)

usage:

python2 ./blast_lines.py -input INPUT [-output OUTPUT] [-ORGANISM taxidOfInterest] [-res_num umberOfResults]

The defaults are:
  
  -ORGANISM txid7227[ORGN] (fly)
  -res_num 20
  
  






