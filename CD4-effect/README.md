# Molecular Dynamics Simulations Reveal Distinct Differences in Conformational Dynamics and Thermodynamics between the Unliganded and CD4-bound States of HIV-1 gp120

## Models
1. unliganded gp120

The [unliganded gp120](./models/unliganded.pdb) structural model was constructed using the homology modeling procedure implemented in MODELLER V9.17. The gp160 sequence of the HIV-1 HXBc2 isolate (clade B) was obtained from UniProtKB database (http://www.uniprot.org) with accession number P04578. Residues of the signal peptide, partial gp120 N-terminus, and gp41 were removed, and the finally obtained gp120 target sequence comprises 462 amino acid residues. The gp120 atomic coordinate extracted from a closed unliganded Env trimer crystal structure (PDB ID: 5FYJ (chain G); 3.11 Å resolution) from HIV-1 clade G was used as the template.

2. CD4-complexed gp120

The [CD4-complexed gp120](./models/CD4-bound.pdb) was extracted from an atomistic model of HIV Env trimer obtained from Protein Data Bank (PDB) (http://www.rcsb.org) with PDB ID 3J70.

## Molecular dynamics (MD) simulation

### Software

All MD simulations were performed using GROMACS V5.1.4.

### Parameter

All parameters related to MD can be find in [gmx_mdp_files](./gmx_mdp_files/).

### Trajectory

Only Cα atoms were extracted from 10 MD simulation replicas and can be find in [trajectory_ca](./trajectory_ca/).

### RMSD & RMSF

The backbone root mean square deviation ([RMSD](./rmsd/)) and Per-residue Cα root mean square fluctuation ([RMSF](./rmsf/)) were calculated using a variety of trajectory analysis tools implemented in GROMACS.