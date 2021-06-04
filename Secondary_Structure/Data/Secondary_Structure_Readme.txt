You can load the dataset using numpy. The code to load the dataset is given below:
data = np.load('Secondary_Structure_Test_Dataset.npz')
sequence = data['sequences']
pssm = data['pssms']
secondary_structure = data['secondaryStrucs']

The shape of numpy array for sequence is (X, 700, 21); here 21 is the number of unique amino acids, which are numbered as follow in one hot encoded form: A, C, E, D, G, F, I, H, K, M, L, N, Q, P, S, R, T, W, V, Y, X (unknown). The shape of pssm is (X, 700, 22) and shape of secondary_structure is (X, 700, 8); here 8 is the number of types of secondary structure, which are numbered as follow in one hot encoded form: L, B, E, G, I, H, S, T. In all arrays X is number of protein sequences, 700 is the maximum length of a protein sequence.


You can load motifs and antimotifs from using numpy. The code to load motifs and antimotifs is given below:
X = np.load('Secondary_Structure_Motif_Antimotif.npz')
motifs = X['motifs']
antimotifs = X['antimotifs']

Both motifs and antimotifs variables are list of motifs and antimotifs found in the train dataset of secondary structure.

