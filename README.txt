## Getting started ##
	1. Unzip the package.
	2. In the directory 'bin', open up a Terminal / Command Line Prompt window.
	3. Run PLW using the following syntax: "./PLW <input.txt> <output_clusters.txt>"
	   For example, to run PLW on the supplied DIP dataset, type the next line (without the quotes):
	   (Linux/Mac)
	   "./PLW ../inputData/ppi.dip.cleaned.txt clusters.txt"
	   (Windows)
	   "PLW ../inputData/ppi.dip.cleaned.txt clusters.txt"
	4. Using this example, PLW will run and produce a tab-delimited file called "clusters.txt" in
	   the same directory containing the predicted complex. Each line of the output file represents
	   a complex, with the first number representing the numeric ID of the complex, the second
	   number representing the number of proteins in the predicted complex, and the remaining
	   line representing the proteins in the complex. A summary of PLW's progress will be sent to
	   stderr.

       Further information on the usage of PLW and its command-line options can be found in
       bin/README.txt.

## File contents of this package ##
|____bin
| |____PLW_MacOSX
| |____PLW_MacOSX_without_OpenMP
| |____README.txt
|____inputData
| |____ppi.combined6.cleaned.txt
| |____ppi.dip.cleaned.txt
| |____README.txt
|____README.txt

bin/: Binaries for PLW
	Instructions on using PLW and its command-line options can be found in bin/README.txt.

## References ##
If you use PLW in your research, we would greatly appreciate it if you cite our paper:

Daniel Lin-Kit Wong, Xiao-Li Li, Min Wu, Jie Zheng and See-Kiong Ng
PLW: Probabilistic Local Walks for Detecting Protein Complexes from Protein Interaction Networks
Working Paper

## Contact us ##
If you have any queries, please email Daniel Wong (wonglkd@gmail.com).