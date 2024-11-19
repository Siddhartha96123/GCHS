# General Conformational Heterogeneity Scanner 1.0 (GCHS_1.0)

## Introduction

Greetings and salutations, fellow *Homo sapiens sapiens*! 🌍

Welcome to the **General Conformational Heterogeneity Scanner (GCHS)**, a Python-based tool designed to compare the structural nuances of two biomolecules in .pdb format. At its core, this tool enables PDB structure alignment and 'Root Mean Square Deviation/residue' (RMSD/res) analysis. It offers a granular perspective of structural differences between biomolecular states, such as apo vs ligand-bound forms or same biomolecules under different conditions.

Whether you are a seasoned structural biologist, a computational enthusiast, or a curious researcher, this tool is designed with simplicity and utility in mind, ensuring you can extract meaningful insights from your structural data.

## Background

This tool was born out of a deep fascination for structural biology and the urge to explore conformational heterogeneity in biomolecular systems. It is inspired by my scientific journey, which began during a research internship at ICGEB, New Delhi, in 2017. There, I was introduced to the fundamentals of the drug discovery pipeline and the role of structural scrutiny in answering key biological questions.

My first scientific research article, "Conformational heterogeneity in apo and drug-bound structures of Toxoplasma gondii prolyl-tRNA synthetase", highlighted the utility of RMSF (RMSD/residue) over elementary RMSD calculations in analyzing biomolecular structures. This work formed the basis of the GCHS tool, which aims to provide a robust, systematic, and visual approach for structural comparisons.

If you're interested, the article is :	

"Mishra, S., Malhotra, N., Kumari, S., Sato, M., Kikuchi, H., Yogavel, M., & Sharma, A.*. (2019). Conformational heterogeneity in apo and drug-bound structures of Toxoplasma gondii prolyl-tRNA synthetase. Acta crystallographica. Section F, Structural biology communications, 75(Pt 11), 714–724."

It's DOI is : https://doi.org/10.1107/S2053230X19014808. 

## Features

- Structural Alignment: Aligns two .pdb files using C-alpha atoms.
- RMSF Analysis: Calculates the Euclidean distances between corresponding C-alpha atoms of aligned residues.
- Granular Insights: Focuses on residue-level differences, providing a per-residue RMSF value for better interpretability.

## Requirements

To use GCHS, ensure you have the following installed:

- Python 3.x
- Biopython: pip install biopython
- pandas: pip install pandas
- openpyxl: pip install openpyxl
- matplotlib: pip install matplotlib

## Usage

### Upload PDB Files:

- Reference PDB: The structure to which the target structure will be aligned.
- Target PDB: The structure to be aligned.

### Structural Alignment:

- Distance Calculation: Computes the Euclidean distances between corresponding C-alpha atoms in aligned structures.
- Data Recording: Record the calculated distances in excel format.

### Visualization: 

Matplot used to plot the recorded distances against the correspondingly aligned residue ID of the Target PDB. 

## Output:

- An Excel file (GCHS_PDB_RMSF.xlsx) with residue pairings and distances.
  - Columns: Reference Residue ID, Aligned Residue ID, RMSF Distance (in Å).
- A scatter plot (GCHS_PDB_RMSF_plot.png) visualizing RMSF values against residue IDs.
  - X-axis: Reference Residue IDs.
  - Y-axis: RMSF values (in Å).

## Limitations

- Currently, the tool supports only PDB files with a single chain.
- For multi-chain structures, split the chains into individual files before analysis.
- Focuses solely on C-alpha atoms for alignment and distance calculation.

# Example Workflow

1. Open the script on a Jupyter notebook environment, preferably "Google Colab" - Script written with its aid.
2. Run the script and upload your reference and target PDB files when prompted.
3. The tool will perform alignment, calculate RMSF values, and generate output files for download.
4. Visualize or analyze the results using the provided outputs.

# Why GCHS?

The GCHS tool provides:

- Granularity: RMSF offers residue-level precision compared to global RMSD.
- Flexibility: Works with any .pdb file containing biomolecular structures.
- Ease of Use: Simple workflow and clear outputs.

It is particularly useful for:

- Comparing apo vs ligand-bound biomolecular states.
- Investigating structural differences under varying experimental conditions.
- Investigating structural differences between orthologous proteins. 
- Exploring conformational heterogeneity for hypothesis generation.

### Acknowledgments

The development of this tool is a reflection of my scientific journey and the invaluable guidance of mentors and collaborators. Special thanks to the Structural and Computational Biology Group at ICGEB, New Delhi, for the foundational knowledge and inspiration.

### Citation

If you use GCHS in your work, please consider citing the aforementioned article.

I am endeavouring to write another article dedicated just for this tool. Once I have it out, will add that onto here too. 

Thank You for your consideration. 

### Get Involved

This is just the beginning! GCHS will continue to evolve, with plans to:

- Extend support for multi-chain PDB files.
- Include RNA and DNA structures for nucleic acid-based comparisons.
- Implement additional features for dynamic trajectory analysis.

## License

This tool is licensed under the MIT License. See the LICENSE file for details.

## Connect

- Email: siddhartha96123@gmail.com
- LinkedIn: linkedin.com/in/siddhartha-mishra-749515125

**Join the journey to revolutionize bioinformatics and structural biology. This is only the beginning!**

***Feel free to fork, contribute, or reach out with feedback and ideas.***  
