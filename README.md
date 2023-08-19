# matplotlib_challenge

### This repo contains the necessary artifacts to satisfy the requirements of this challenge.

| File | Description | 
| - | - |
| `Pymaceuticals/data/Mouse_metadata.csv` | Dataset representing the mouse data for the challenge. |
| `Pymaceuticals/data/Study_result.csv` | Dataset representing the clinical trial data for the challenge. |
| `Pymaceuticals/pymaceuticals.ipynb` | Jupyter Notebook file that contains the code to complete the challenge as well as the written analysis. |

# Analysis

This analysis report is also found in the Jypyter Notebook, but is included here as well for convenience.

- When comparing Capomulin to the rest of the drugs in the study, Capomulin better than all other drugs with the exception of Ramicane in terms of average tumor size at the end of the study.  Only Capomulin and Ramicane actually saw a reduction in tumor size, since all specimens started with 45.0 mm3 tumor volume.
	
|Drug Regimen |mean	|median	|std|	
|-|-|-|-|		
|Ramicane	|36.191390	|36.561652	|5.671539|
|Capomulin	|36.667568	|38.125164	|5.715188|
|Propriva	|56.493884	|55.591622	|8.415626|
|Ceftamin	|57.753977	|59.851956	|8.365568|
|Infubinol	|58.178246	|60.165180	|8.602957|
|Zoniferol	|59.181258	|61.840058	|8.767099|
|Placebo	|60.508414	|62.030594	|8.874672|
|Stelasyn	|61.001707	|62.192350	|9.504293|
|Naftisol	|61.205757	|63.283288	|10.297083|
|Ketapril	|62.806191	|64.487812	|9.945920|

(source: average_tumor_size_at_end_by_drug DataFrame)

- When comparing the mouse's weight to the tumor size, for the Capomulin drug, there was a strong correlation (r = 0.84) between these variables.  So the heavier the mouse is, the larger the tumor.