PLW: Probabilistic Local Walks
==============================

Getting started
---------------

1. Unzip the package.
2. In the directory 'bin', open up a Terminal / Command Prompt window.
3. Run PLW using the following syntax: `./PLW <input.txt> <output_clusters.txt>`  

   For example, to run PLW on the supplied DIP dataset, type the next line:  
   **Mac**:
   ```./PLW_MacOSX ../inputData/ppi.dip.cleaned.txt clusters.txt```  
   **Linux**:
   ```./PLW_Linux ../inputData/ppi.dip.cleaned.txt clusters.txt```  
   **Windows**:
   ```PLW_Win ..\inputData\ppi.dip.cleaned.txt clusters.txt```  
   **Windows (with Cygwin)**:
   ```PLW_Win_cygwin ../inputData/ppi.dip.cleaned.txt clusters.txt```

4. Using this example, PLW will run and produce a tab-delimited file called `clusters.txt` in
   the same directory containing the predicted complex. Each line of the output file represents
   a complex, with the first number representing the numeric ID of the complex, the second
   number representing the number of proteins in the predicted complex, and the remaining
   line representing the proteins in the complex. A summary of PLW's progress will be sent to
   `stderr`.

	Further information on the usage of PLW and its command-line options can be found in
	`bin/README.txt`.

Package contents
----------------
 * `bin`
    * `PLW_MacOSX`
    * `PLW_Linux`
    * `PLW_Win.exe`
    * `PLW_Win_cygwin.exe`
    * `README.txt`
 * `inputData`
    * `ppi.combined6.cleaned.txt`
    * `ppi.dip.cleaned.txt`
    * `README.md`
 * `README.txt`

Instructions on using PLW and its command-line options can be found in `bin/README.txt`.

References
----------
If you use PLW in your research, we would greatly appreciate it if you cite our paper:

Daniel Lin-Kit Wong, Xiao-Li Li, Min Wu, Jie Zheng and See-Kiong Ng  
**PLW: Probabilistic Local Walks for Detecting Protein Complexes from Protein Interaction Networks**  
*BMC Genomics* 2013 Volume 14 (Suppl 5), S15.  
http://www.biomedcentral.com/1471-2164/14/S5/S15  
Presented in the *International Conference on Bioinformatics 2013* (InCoB2013).

BibTeX
------

    @article{Wong2013PLW,
      title={PLW: Probabilistic Local Walks for detecting protein complexes from protein interaction networks},
      author={Daniel Lin-Kit Wong and Li, Xiao-Li and Wu, Min and Zheng, Jie and Ng, See-Kiong},
      journal={BMC Genomics},
      doi = {10.1186/1471-2164-14-s5-s15},
      url = {http://dx.doi.org/10.1186/1471-2164-14-s5-s15},
      volume={14},
      number={Suppl 5},
      pages={S15},
      year={2013},
      publisher={BioMed Central Ltd},
      pmid = {24564427},
      issn = {1471-2164},
      abstract = {{BACKGROUND: Many biological processes are carried out by proteins interacting with each other in the form of protein complexes. However, large-scale detection of protein complexes has remained constrained by experimental limitations. As such, computational detection of protein complexes by applying clustering algorithms on the abundantly available protein-protein interaction (PPI) networks is an important alternative. However, many current algorithms have overlooked the importance of selecting seeds for expansion into clusters without excluding important proteins and including many noisy ones, while ensuring a high degree of functional homogeneity amongst the proteins detected for the complexes.

      RESULTS: We designed a novel method called Probabilistic Local Walks (PLW) which clusters regions in a PPI network with high functional similarity to find protein complex cores with high precision and efficiency in O(|V| log |V| + |E|) time. A seed selection strategy, which prioritises seeds with dense neighbourhoods, was devised. We defined a topological measure, called common neighbour similarity, to estimate the functional similarity of two proteins given the number of their common neighbours.

      CONCLUSIONS: Our proposed PLW algorithm achieved the highest F-measure (recall and precision) when compared to 11 state-of-the-art methods on yeast protein interaction data, with an improvement of 16.7\% over the next highest score. Our experiments also demonstrated that our seed selection strategy is able to increase algorithm precision when applied to three previous protein complex mining techniques.AVAILABILITY:The software, datasets and predicted complexes are available at http://wonglkd.github.io/PLW}}
    }

Contact us
----------
More information can be found at the project website at <http://wonglkd.github.io/PLW>.  
If you have any queries, please email Daniel Wong at <wonglkd@gmail.com>.
