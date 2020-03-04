# PedMix: software for ancestral inference of single admixed individual

Software accompnay for "Inferring the ancestry of parents and grandparents from genetic data", by Jingwen Pei, Yiming Zhang, Rasmus Nielsen and Yufeng Wu, submitted for publication, 2020.
This paper is currently under review. An early version is available at bioRxiv: https://www.biorxiv.org/content/10.1101/308494v1

PedMix is a software tool for inferring the admixture proportions of recent ancestors (e.g., parents, grandparents or great-grandparents) of a focal individual. The input for PedMix is the phased haplotypes of an diploid individual. Pedmix can infer the admixture proportions of ancestors, not the focal individual. To fix ideas, suppose an individual has genes from ancestral populations A and B. Existing genetic testing approaches can infer the admixture proportions of this focal individual. PedMix, instead, infers the admixture proportions of parents or other recent ancestors (e.g. what are the percentages of genes the two parents inherit from A and B?).

Please read the user manual to get started on PedMix.

For your convenience, I have posted an executable of PedMix for Linux 64 bits. However, I recommend you to consider building PedMix from source code (posted here). You will need to install a library for BFGS optimization from: https://github.com/chokkan/liblbfgs

# Utilities
We provide two utility programs which we have found to be useful.
(1) Frequency-based pruning (in the Pruning.zip file). This simple tool prunes the input haplotypes to remove SNPs that may not be very informative for ancestral infernece. Our experience indicates that this kind of pruning not only speeds up the computation, but also can improve the inference accuracy.
(2) Phasing error correction (in the PhasingCorrection.zip file). This simple tool is designed to remove phasing errors from the input haplotypes. Our experience suggests that this tool can help to improve the inference accuracy (sometime by quite a bit).

If you have questions, please email: yufeng.wu@uconn.edu.

# Note:
PedMix has been distributed in GitHub earlier at: https://github.com/pjweggy/PedMix by my former student, Jingwen Pei.
Since Jingwen has left my research group, I decide to create a new repository for better maintance of the code.
