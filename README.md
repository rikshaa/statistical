### Identification Procedure

Identification was performed by creating a "database" which stored all the FC matrices of each individual from session 1. Iteratively, the FC matrix from a given individual from session 2 was then selected and this FC matrix was treated as the "target matrix". The target matrix was then compared with each of the FC matrices in the database to find the corresponding matrix which is maximally correlated with each other. An individual is correctly identified if the FC matrices in the database and target matrix share the highest Pearson's correlation coefficient. The predicted identity (ID) was compuated using two approaches:
1. binary identification (BID): ID was assigned a score of 1 if the predicted identity matched the true identity of the individual, otherwise the ID was given a score of 0.
2. relative rank (RR): RR is a continuous measure ranging from 0 to 1, and quantifies the degree of "confusion" for inaccurately identified individuals such that the fewer individuals inaccurately ranked above their true ID, the lower the degree of confusion and lower the RR.

The ID accuracy for each dataset was computed as the percentage of individuals who were correctly identified out of the total number of individuals in each dataset. We then averaged the ID accuracy for each dataset by exchanging the roles of the database-target matrix. The identification procedure was repeated until the FC matrices of each subject served as target matrices across the five datasets and two database-target matrix configurations.

### Head Motion

Failure to control for gross motion has the potential to bias the true estimates of FC-based measures as there is an inverse relationship between FC patterns and head movements, especially in developmental cohorts [(Satterthwaite et al., 2012)](https://pubmed.ncbi.nlm.nih.gov/22233733/). In order to avoid head motion in confounding the ID accuracy, we excluded high-motion individuals in the five datasets by using a root-mean-square framewise displacement (rmsFD) threshold as implemented by [Jenkinson et al. (2002)](https://pubmed.ncbi.nlm.nih.gov/12377157/). We selected an rmsFD threshold that is neither very strict (e.g. rmsFD < 0.1mm) nor very liberal (e.g. rmsFD > 0.3-0.5mm). We retained all the low-motion individuals with rmsFD <= 0.2mm in either imaging session. We then determined whether there was a relationship between head motion and ID accuracy in both imaging sessions.

### Structural & Functional Data

Structural and functional data were obtained from the openly available [Consortium for Replicability and Reproducibility (CoRR)](http://fcon_1000.projects.nitrc.org/indi/CoRR/html/samples.html) spanning childhood to adulthood. A total of five independent datasets were used which include the New York University (NYUadu), New York University (NYUado), University of Pittsburgh School of Medicine (UPSM), Beijing Normal University (BNU) and Southwest University (SWU). For each dataset, two resting-state scans were obtained from two imaging sessions either on the same day or after several months and years. The complete information regarding the demographic details and fMRI acquisition parameters are provided below.

|  Dataset    |  NYUadu    | NYUado   | UPSM   | BNU   | SWU   |
| :---    |  :---: |  :---: | :---:|:---:|:---:|
| Sample Size | 31 | 25 | 67 | 60 | 82 |
| Age Range (years) | 18-43 | 7-13 | 14-19 | 19-23 | 18-25 |
| Gender (M:Male F:Female) | M:16 F:15 | M:15 F:10 | M:34 F:33 | M:32 F:28 | M:33 F:49 |
| Scan Duration (min) | 06:00 | 06:00 | 05:06 | 08:06 | 08:00 |
| Time Between Retest Scans | Same day | Same day | 1-4 years | 3 months | 1 year |
| Scanner Manufacturer | Siemens | Siemens | Siemens | Siemens | Siemens |
| Scanner Model | Magnetom Allegra | Magnetom Allegra | TrioTrim | TrioTrim | TrioTrim |
| Field Strength | 3.0T | 3.0T | 3.0T | 3.0T | 3.0T | 
| TR (ms) | 2000 | 2000 | 1500 | 2000 | 2000 |
