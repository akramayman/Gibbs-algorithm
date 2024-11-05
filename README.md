# Gibbs-algorithm

## Motif finding By Gibbs sampling algorithm.

This project is talking about Gibbs sampler method, which is a statistical method that is built based on the probability of nucleotide position. The method depends on specific number of nucleotides from the original sequence to find motifs, which are recurring patterns in DNA that presumed to have a biological function. We used C++ language in our project. In genetics, a sequence motif is a nucleotide or amino-acid sequence pattern that is widespread and has, or is conjectured to have, a biological significance. For proteins, a sequence motif is distinguished from a structural motif, a motif formed by the three-dimensional arrangement of amino acids which may or may not be adjacent. When motif sequence appears in the exon of  gene, it may encode the "structural motif " of a protein. We validated our result analytically and the accuracy and the speed were high as shown in the results section.

Gibbs sampler is a Markov chain Monte Carlo (MCMC) algorithm for obtaining a sequence of observations which are approximately from a specified multivariate probability distribution, when direct sampling is difficult,there are five steps in Gibbs sampler we follow to get the motif which are component of matrices that depends on statistical and computational operations.

## 1) Initialization
In this step we choose initial random position of motif, then we reject one sequence at each iteration and this one is the sequence that we find the motif position for it.

## 2) Profile matrix
In this matrix we calculate the background which is the frequency of nucleotide that remains out of random sequences.

## 3) Predictive update step
Update proﬁle matrix based on motif and background frequencies and pseudocounts which is a small number that we add to the calculation to avoid multiplying and divided by zero.
![image](https://github.com/user-attachments/assets/f656c4aa-bb72-4bd3-8ba6-59be2cb2360a)
![image](https://github.com/user-attachments/assets/408c209e-c447-4e78-a8cd-3d07fa81a70c)

## 4) Sampling step
For each possible motif start position, we calculate the ratio of likelihood of next positions from motif vs. background.
![image](https://github.com/user-attachments/assets/501677b6-7f0e-4f6d-a2c2-3bb46a35a52b)

## 5) Normalization


## Requirements to run the code:
### 1) choose sequences with length 10 nucleotides.
can take for example these sequences:
ACCATGACAG
GAGTATACCT
CATGCTTACT
CGGAATGCAT

### 2) choose random initial position of motif



