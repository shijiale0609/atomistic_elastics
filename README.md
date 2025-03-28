# atomistic_elastics
This repository contains supplementary forcefields, topologies, and runfiles in the paper 

**Automated determination of n-cyanobiphenyl and n-cyanobiphenyl binary mixtures elastic constants in the nematic phase from molecular simulation** by Jiale Shi, Hythem Sidky, Jonathan K Whitmer Mol. Syst. Des. Eng., 2020, 5, 1131-1136 [Link](https://pubs.rsc.org/en/content/articlehtml/2020/me/c9me00065h)


## What's inside? 
- Gromacs topologies, configurations, and run parameters.
- Representative SSAGES input file for elastic free energy measurement.
- Python scripts used in workflow to generate run files across temperature ranges. 

The **bulk** folder contains an equilibrated configuration used for bulk 
elastic measurements (k_ii). The **cylinder** folder contains an equilibrated
configuration of cylindrically confined 5CB for k_24 measurements.

## The updates between this repo and https://github.com/hsidky/atomistic_elastics.git 

https://github.com/hsidky/atomistic_elastics.git is about this work **In Silico Measurement of Elastic Moduli of Nematic Liquid Crystals** by Hythem Sidky,Juan J. de Pablo and Jonathan K. Whitmer.

- This repo uses ABF (Adaptive Biasing Force Algorithm) instead of BFS (Basis Function Sampling) for calculating elastic constants (gen_elastic_runs.py). 
- This repo adds forcefield for 6CB, 7CB, 8CB, and 5CB/8CB(0.50/0.50)
- This repo adds bulk input files for 6CB, 7CB, 8CB, and 5CB/8CB(0.50/0.50)

## Notes:
- This work needs a CV called nematic order, which is contained in a specific version of SSAGES in [SSAGESv6](./SSAGESv6). 
