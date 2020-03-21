# Molecular dynamics simulations reveal distinct differences in conformational dynamics and thermodynamics between the unliganded and CD4-bound states of HIV-1 gp120

## Abstract

The entry of human immunodeficiency virus type I (HIV-1) into host cells is initiated by binding to the cell-surface receptor CD4, which induces a conformational transition of the envelope (Env) glycoprotein gp120 from the closed, unliganded state to the open, CD4-bound state. Despite many available structures in these two states, detailed aspects on the dynamics and thermodynamics of gp120 remain elusive. Here, we performed s-scale multiple-replica molecular dynamics (MD) simulations to explore the differences in the conformational dynamics, protein motions, and thermodynamics between the unliganded and CD4-bound/complexed forms of gp120. Comparative analyses of MD trajectories reveal that CD4 binding promotes the structural deviations/changes and conformational flexibility, loosens the structural packing, and complicates the molecular motions of gp120. Comparison of the constructed free energy landscapes (FELs) reveals that the CD4-complexed gp120 has more conformational substates, larger conformational entropy, and lower thermostability than the unliganded form. Therefore, the unliganded conformation represents a structurally and energetically stable “ground state” for the full-length monomeric gp120. The observed great increase in the mobility of V1/V2 and V3 along with their more versatile movement directions in the CD4-bound gp120 compared to the unliganded form suggests that their orientations with respect to each other and to the structural core determine the differences in the conformational dynamics and thermodynamics between the two gp120 forms. The results presented here provide a basis by which to better understand the functional and immunological properties of gp120 and, furthermore, to deploy appropriate strategies for the development of anti-HIV-1 drugs or vaccines.

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