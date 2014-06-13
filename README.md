PooLD
Increasing the effective coverage in Pooled sequencing using LD

Currently, methods for detect SNPs under selection in "evolve & re-sequence" experiments analyze each SNP separately. For example, ?DiffStat? is used to determine whether allele frequencies in the experimental evolved populations differ significantly from simulated allele frequencies. Other methods include Fisher?s exact test, chi-squared test, and an a posteriori Dunnett test which are used to detect significant allele frequency differences between treatments. All of these methods are ignoring the often available haplotype panels that contains information on SNP correlations. Although, recently a method by Kessner et al, reconstruct the haplotypes using the haplotype panel but this method is window-based and relies on the assumption that the haplotypes in the evolved population are near perfect mosaics of the haplotype panel which in our data is not true.

Our aim is to use this information to increase the effective coverage for each SNP. The intuition is that the haplotype panel allows computation of SNP correlations which then allows the use of correlated reads in estimating the frequency of a particular SNP. For example with two perfectly correlated SNPs, one can utilize information from both SNPs to double the coverage at any one SNP.