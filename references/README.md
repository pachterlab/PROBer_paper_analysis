#### Arabidopsis reference

1. There are two copies of 18S rRNA, `AT2G01010.1` and `AT3G41768.1`. `AT2G01010.1` is consistent with the ground truth 18S sequence from [RNA structure database](http://www.rna.icmb.utexas.edu/DAT/3B/Standard/index.php?xysub=1&organism=Arabidopsis%20thaliana&seq_size=&rna_type=&orf=&rna_class=&from_gene=&structure=ALL&cell_loc=&ord=&xyac_info=m&xybegin=0&xyrange=50&xyco=yes&query_type=results) and `AT3G41768.1` is not. Thus, `AT3G41768.1` is removed.

2. The large subunit sequence from [RNA structure database](http://www.rna.icmb.utexas.edu/DAT/3B/Standard/index.php?xysub=1&organism=Arabidopsis%20thaliana&seq_size=&rna_type=&orf=&rna_class=&from_gene=&structure=ALL&cell_loc=&ord=&xyac_info=m&xybegin=0&xyrange=50&xyco=yes&query_type=results) contains both 5.8S and 25S sequences. Because 5.8S (`AT2G01020.1`) existed in the reference, we splitted the large subunit sequence and only add the 25S part into the reference.

#### Yeast reference

1. The following rRNAs are removed: `RDN37-1`, `RDN37-2`, `RDN18-2`, `RDN25-2`, `RDN58-2`, `RDN5-2`, `RDN5-3`, `RDN5-4`, `RDN5-5` and `RDN5-6`. Note that RDN37 is the combination of 5.8S, 18S and 25S rRNAs.

2. `YLR154C-G`, which is part of `RDN5-2`, is also removed.

#### Mouse reference

The mouse annotation contains 353 variants of 5S rRNA. We only kept one variant(`n-R5S100`), which is contained in both Ensembl and RefSeq annotations.