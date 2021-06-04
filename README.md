# Applications-of-NLP-techniques-in-Biology

This repository contains the Data, Code, and Weights to replicate the results of the proposed models in the paper titled: **Applications of NLP techniques in Biology**.
The two folders in the repository are for the two different sequence to sequence problems used in the paper.

- ### Secondary Structure
In this problem, we need to classify each amino acid in the protein sequence into a type of secondary structure.
There are 8 different type of secondary structure: &beta;-Sheet (E), &beta;-Bridge (B), &alpha;-Helix (H), &pi;-Helix (I), 3<sub>10</sub>-Helix (G), Irregular (L), Bend (S), Turn (T).

The folder Secondary_Structure contains the following:
- Notebooks of the proposed models.
- Folder named Data, which contains to training and test datasets along with a list of class based motifs and anti-motifs found in the training dataset. It also contains a readme about the files in the folder.
- Folder named Weights, which contains trained weights of the proposed models.

- ### Disordered Regions
In this problem, for each amino acid in the protein sequence, we need to classify whether in 3-D it will be in ordered or disordered shape.

The folder Disordered_Regions contains the following:
- Notebooks of the proposed models.
- Folder named Data, which contains to training and test datasets along with a list of class based motifs and anti-motifs found in the training dataset of the secondary structure problem. It also contains a readme about the files in the folder.
- Folder named Weights, which contains trained weights of the proposed models.

