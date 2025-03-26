# wgsim

[wgsim](https://github.com/lh3/wgsim), qui fait partie de l'outil [SAMtools](https://www.htslib.org/), est un simulateur de séquences de lecture pour des données de séquençage. Il est conçu pour simuler des lectures de séquençage à partir d'un génome de référence, ce qui peut être utile pour tester des outils bioinformatiques ou pour évaluer la performance de méthodes d'alignement et d'assemblage.

```
Program: wgsim (short read simulator)
Version: 1.9
Contact: Heng Li <lh3@sanger.ac.uk>

Usage:   wgsim [options] <in.ref.fa> <out.read1.fq> <out.read2.fq>

Options: -e FLOAT      base error rate [0.020]
         -d INT        outer distance between the two ends [500]
         -s INT        standard deviation [50]
         -N INT        number of read pairs [1000000]
         -1 INT        length of the first read [70]
         -2 INT        length of the second read [70]
         -r FLOAT      rate of mutations [0.0010]
         -R FLOAT      fraction of indels [0.15]
         -X FLOAT      probability an indel is extended [0.30]
         -S INT        seed for random generator [0, use the current time]
         -A FLOAT      discard if the fraction of ambiguous bases higher than FLOAT [0.05]
         -h            haplotype mode
```