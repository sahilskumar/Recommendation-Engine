Data : http://www.kaggle.com/benhamner/nips-papers
Paper : http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.75.3005&rep=rep1&type=pdf

//Recommendation engine above implemented is Content Based recommends only using information about the items being recommended. 
  There is no information about the users.
  
 PROCEDURE
  LSH Checklist
As a final checklist for performing LSH, ensure that you complete the following steps:

1. Create shingles from your available data set (e.g. unigrams, bigrams, ratings, etc.)
2. Build an m×n shingle matrix where every shingle that appears in a set is marked with a 1 otherwise 0.
3. Permute the rows of the shingle matrix from step 2 and build a new p×n signature matrix where the number of the 
   row of the first shingle to appear for a set is recorded for the permutation of the signature matrix.
4. Repeat permuting the rows of the input matrix times and complete filling in the p×n signature matrix.
5.Choose a band size b for the number of rows you will compare between sets in the LSH matrix.
