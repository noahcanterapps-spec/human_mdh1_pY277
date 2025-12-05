# Homo sapiens MDH1

# Uniprot ID: P40925
# Variation: phosphorylation of Y277 (pY277)


## Description

Tyrosine 277 of human MDH1 is not documented as a known post-translational modification site in UniProt, PhosphoSitePlus, or the primary literature. However, the position lies on a surface loop near residues that border the substrate-binding cleft. Given its proximity to residues involved in stabilizing malate and NAD⁺, modification at this position could significantly alter local electrostatics, loop mobility, or substrate access. Although no experimental studies describe this specific PTM, structural modeling enables prediction of how phosphorylation or acidic substitution may influence enzyme function and metabolic flux through the malate–aspartate shuttle.

*Entry started 12/04/2025 NC*

# Comparison of MDH1 models and phospho modified MDH1

1. Alignment of MDH1, MDH1-pY277 (orange), and MDH1-Y277D (magenta)  
![Alignment of MDH1, MDH1-pY277, and Y277D](site_compare_p277.png){: width="300px"}

2. Modification site alignment within MDH1  
![Modification site alignment](site_modified_pY277.png)

The modification site is close to Asn275, Ser276, Gly278, and Arg309. Phosphorylation introduces a bulky dianionic phosphate, which creates new electrostatic contacts with Arg309 and Glu300 while disrupting hydrophobic packing around residues 275–304. The mimetic substitution (Y277D) introduces only a single negative charge and lacks the steric bulk of the phosphate, resulting in a different interaction pattern and increased local disorder.

---

## Effect of the sequence variant and PTM on MDH dynamics

The RMSD after molecular dynamics-style elastic network simulation indicates modest structural divergence between unmodified and mimic structures. The unmodified MDH1 is shown in green while Y277D is in purple.

![MD alignment plot](rmsf_plot_mdh1_pY277.png)

After simulation, residues surrounding the 277-containing loop (residues 275–304) show higher RMSF in the Y277D simulation, indicating increased mobility and loss of stabilizing contacts normally present in the native structure. These changes propagate toward the substrate-binding cleft.

![Modification-site MD view](site_mimic_y277d.png)

### Comparison of the enzyme dynamics

The RMSF plot shows increased dynamics around residues 275–304. These loops border the region that repositions during malate/NAD⁺ binding. Increased local motion could destabilize catalytic alignment or affect substrate residence time.

![RMSF comparison](rmsf_plot_mdh1_pY277.png)

### Effect of modification on the pKa values

Overall, the mimic modification influences the electrostatic microenvironment near residue 277. pKa predictions show small but consistent shifts in charged residues near the site (Asp275, Glu300, Arg309). These changes reflect altered stabilization of ionizable groups caused by the negative charge at position 277.

(pKa data files included: `pkas_over_traj.csv`, `pkas_describe.csv`)

---

## Comparison of the mimic and the authentic PTM

The Y277D phosphomimetic variant does **not** fully reproduce the behavior of the phosphorylated tyrosine. While both introduce negative charge, the phosphate moiety produces steric bulk and multiple directional hydrogen bond donors/acceptors, enabling interactions not possible with Asp. The modified (pY277) structure forms a stabilized electrostatic hub with Arg309 and Glu300, producing loop rigidification. In contrast, the Y277D variant introduces greater disorder and fewer stabilizing contacts.

![Comparison of PTM vs mimic](site_compare_p277.png)

---

### Colab notebook links

Files produced using Colab MD simulation:  
- `ensemble.pdb`  
- `rmsf_df.csv`  
- `rmsf_plot_mdh1_pY277.png`  
- `pkas_over_traj.csv`  
- `pkas_describe.csv`  

---

## Authors

Noah Canter

## Deposition Date
12/04/2025

## License

Shield: [![CC BY-NC 4.0][cc-by-nc-shield]][cc-by-nc]

This work is licensed under a  
[Creative Commons Attribution-NonCommercial 4.0 International License][cc-by-nc].

[![CC BY-NC 4.0][cc-by-nc-image]][cc-by-nc]

[cc-by-nc]: https://creativecommons.org/licenses/by-nc/4.0/  
[cc-by-nc-image]: https://licensebuttons.net/l/by-nc/4.0/88x31.png  
[cc-by-nc-shield]: https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey.svg

## References

* UniProt Consortium. “UniProt: A Worldwide Hub of Protein Knowledge.” *Nucleic Acids Research.*  
* PhosphoSitePlus database (Cell Signaling Technology).  
