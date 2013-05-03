## Usage ##
	./PLW <PPI_edge_list.txt> <Output_Clusters.txt>

## Example ##
	./PLW ../inputData/ppi.dip.cleaned.txt clusters.txt

## Essential options ##
  <position 1>   	                    	PPI edge list (tab-delimited)
  <position 2> 	    		            	Output cluster file location
  --help                                	Produce this help message

## Notes on OpenMP support ##
By default, PLW is able to take advantage of multi-core processors to speed
up the calculation of scores. Parallelisation support for the other calculations,
such as similarity calculation and core mining, is being explored and will be added
in the near future.

## Basic options ##
  -u [ --seedselect_threshold ] arg
                                        	Fraction of Top-Ranked Nodes to use 
                                        	as Seeds [0.0-1.0] [=0.3]
  --randWalk_starting_energy arg        	Core - Random Walk - Starting Energy 
                                        	[=2.0]
  --randWalk_n_walks arg                	Core - Random Walk - No. of walks to 
                                        	take [=100]
  -C [ --core_threshold ] arg 		     	Core Mining Threshold (significance 
                                        	level in term of sigma [=2.5758]
  -P [ --dump_pcores ] arg              	Output processed cores to supplied filename

## Import / Export Data options ##
  -l [ --load_similarities ] arg        	Similiarity Filename to preload
  -L [ --load_scores ] arg              	Score Filename to preload
  -C [ --dump_cores ] arg               	Output unprocessed cores to filename
  -P [ --dump_pcores ] arg              	Output processed cores to supplied filename
  -d [ --dump_similarities ]            	Dump similarities to stdout and exit
  -D [ --dump_scores ]                  	Dump scores to stdout and exit

## Advanced options ##
  --similarity_method arg        			Similarity Method [cos*, cosW, none]
  -s [ --score_method ] arg        			Scoring Method [1-8] [=1]
  -c [ --core_method ] arg			     	Core Method [randWalk*, coach]
  -p [ --process_method ] arg
                                        	Processing Method [rfilter*, none]
  -a [ --attachment_method ] arg
                                        	Attachment-Selection Method [coach*, EM,
                                        	cluster2PrtnLinks, none]
  --randWalk_drop_power arg             	Core - Random Walk - Power to raise the
                                        	drop to [=1]
  -b [ --belonging_threshold ] arg
                                        	Belonging Threshold for adding 
                                       	 	Attachments [0.0-1.0] [=0.50]
  -r [ --redundancy_threshold ] arg)
                                        	Redundancy Threshold for filtering 
                                        	duplicate complexes [0.0-1.0] [=1.0]
  -m [ --merging_threshold ] arg    		Merging Threshold for merging complexes
                                        	[0.0-1.0] [=1.0]
  -v [ --verbose ]                      	Verbose output for debugging
