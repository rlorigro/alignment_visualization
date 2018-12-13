# alignment_visualization
Visualize how reads align to a reference

## Contig or long read mapping visualization

Suppose you have just generated an assembly and aligned it to a true reference, you may want to see the identity of these contigs, and how they map to each chromosome:

![example visualization](https://github.com/rlorigro/alignment_visualization/raw/master/plots/polished_racon_r94_ec_rad2_30x_VS_refEcoli.sorted.png)

Here forward (teal) and reverse (orange) contig alignments are shown. In this case the genome is circular (E. Coli) and there are un-alignable regions of the contig so it is broken up into supplemental alignments. The true chromosome is shown in gray.

The identity measured as `(2*length - 2*n_mismatches - n_deletes - n_inserts) / (2*length)` is shown for each contig, as well as a weighted average denoted by "TOTAL"
