# LSH-for-Product-Duplication
This project uses LSH to identify duplicate products among 1624 televisions based on their product titles.
The structure of the code is as follows:
Data preprocessing, creating the input matrix, performing minhashing, creating a signature matrix and performing LSH on this.
Following this evaluation measures are evaluated for different band lengths. 
Next Jaccard and Signature similarity are computed which are used as input measures for a classifier.

The code can be used with the json file containing the data of all televisions.
The code must be run in order as functions are created from top to bottom.
To adjust the number of bands the value of 50 in the following statement can be adjusted: all_bands = np.vsplit(signature_matrix,50)
Additionally, the threshold for classification is changed manually, currently set at 0.9.

