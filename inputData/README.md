Input Data
==========

Format of files
---------------
* Protein-Protein Interaction Networks `ppi.*.txt`
	* These are tab-delimited edgelists with one edge on each line,
          i.e.: `source<target>destination`
	* These are undirected and unweighted graphs.
	* Cleaned `ppi.*.cleaned.txt`
            * This means that all duplicate edges and self-loops were removed from the graph,
              and the list of edges was sorted alphabetically.

Contents
--------
This directory contains 2 files:

1. ppi.dip.cleaned.txt
	* 4,930 proteins; 17,201 interactions
	* From the Database of Interacting Proteins
		1.	Xenarios I, Salwinski L, Duan X, Higney P, Kim S, Eisenberg D: DIP,
			the Database of Interacting Proteins: a Research Tool for Studying Cellular Networks of
			Protein Interactions. Nucleic Acids Research 2002, 30:303–305.
2. ppi.combined6.cleaned.txt
	* 3,861 proteins; 17,327 interactions
	* Extracted from datasets used by Liu et al. (2009)
	    1.  Liu, Guimei, Limsoon Wong, and Hon Nian Chua.
	    	"Complex discovery from weighted PPI networks."
	    	Bioinformatics 2009, 25(15):1891-1897.
	* Combined from six experiments:
		1.	Ho Y, Gruhler A, Heilbut A, Bader GD, Moore L, Adams SL, Millar A, Taylor P,
			Bennett K, Boutilier K, Yang L, et al: Systematic Identification of Protein Complexes
			in Saccharomyces Cerevisiae by Mass Spectrometry. Nature 2002, 415(6868):180–183.
		2.	Gavin AC, Bosche M, Krause R, Grandi P, Marzioch M, Bauer A, Schultz J, Rick JM,
			Michon AM, Cruciat CM, et al: Functional Organization of the Yeast Proteome by
			Systematic Analysis of Protein Complexes. Nature 2002, 415(6868):141–147.
		3.	Gavin A, Aloy P, Grandi P, Krause R, Boesche M, Marzioch M, Rau C, Jensen LJ, Bastuck S,
			Dumpelfeld B, et al.: Proteome Survey Reveals Modularity of the Yeast Cell Machinery.
			Nature 2006, 440(7084):631–636.
		4.	Krogan N, Cagney G, Yu H, Zhong G, Guo X, Ignatchenko A, Li J, Pu S, Datta N,
			Tikuisis AP, Punna T, et al: Global Landscape of Protein Complexes in the Yeast
			Saccharomyces Cerevisiae. Nature 2006, 440(7084):637–643.
		5.	Uetz P, Giot L, Cagney G, Mansfield TA, Judson RS, et al: A Comprehensive Analysis of
			Protein-Protein Interactions in Saccharomyces Cerevisiae. Nature 2000, 403(6770):623–627.
		6.	Ito T, Chiba T, Ozawa R, Yoshida M, Hattori M, Sakaki Y: A Comprehensive Two-Hybrid
			Analysis to Explore the Yeast Protein Interactome. Proceedings of the National Academy
			of Sciences 2001, 98(8):4569–4574.
