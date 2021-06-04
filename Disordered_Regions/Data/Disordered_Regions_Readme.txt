You can load the dataset using numpy. The code to load the dataset is given below:
data = np.load('Disordered_Regions_Test_Dataset.npz')
sequence_id = data['seq_ids']
sequence = data['sequences']
pssm = data['pssms']
disordered_region = data['regions']

The shape of numpy array for sequence is (X, 1864, 24); here at 0 is append, followed by 20 amino acids (which are numbered as follow in one hot encoded form: A, C, E, D, G, F, I, H, K, M, L, N, Q, P, S, R, T, W, V, Y), than X (unknown), second last indicating start of sequence and last one indicates end of sequence. The shape of pssm is (X, 1864, 20) and shape of disordered_region is (X, 1864, 2); here at 0 ordered region is labeled and disordered at 1. In all arrays X is number of protein sequences, 1864 is the maximum length of a protein sequence. The sequence_id is of length X and contains the id of protein sequence at index i in other arrays.

DM1229_id.txt: This file contain ids of protein sequences in validation dataset.
DM3000_id.txt: This file contain ids of protein sequences in training dataset.
SL329_id.txt: This file contain ids of protein sequences in test dataset.


You can load motifs and antimotifs from using numpy. The code to load motifs and antimotifs is given below:
X = np.load('Secondary_Structure_Motif_Antimotif.npz')
motifs = X['motifs']
antimotifs = X['antimotifs']

Both motifs and antimotifs variables are list of motifs and antimotifs found in the train dataset of secondary structure.
