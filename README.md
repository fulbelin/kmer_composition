# kmer_composition
De Bruijn graph-based assembly technique to reconstruct the original string from the generated k-mers.

K-mer Composition and String Reconstruction
Introduction
This repository focuses on the generation of k-mers from a DNA sequence and the subsequent reconstruction of the original string using these k-mers. The code provided in this repository accomplishes this task for various values of k, including 3, 4, 5, 20, 30, and 50. Additionally, it features an implementation of a function reconstruct_string_from_kmers that utilizes a simplified De Bruijn graph-based assembly technique to reconstruct the original string from the generated k-mers.

Instructions
a. Generating K-mers
Create a DNA sequence of length 100 as an example.
Generate k-mers for each of the following k values: 3, 4, 5, 20, 30, 50.
b. Reconstructing the Original String
Utilize the reconstruct_string_from_kmers function to reconstruct the original string from the generated k-mers.
Implementation Details
c. Explanation of Implementation
The implementation employs a simplified De Bruijn graph-based approach to reconstruct the original string from the generated k-mers. The process involves creating k-mers from a randomly generated DNA sequence and constructing a De Bruijn graph representation. In this graph, nodes represent (k-1)-mers, and edges represent overlapping k-mers. The algorithm aims to find an Eulerian path in this graph, which corresponds to a path traversing every edge exactly once. The reconstructed string is then obtained by concatenating the last character of the last node and the first character of each node in the Eulerian path.

Results and Discussion
d. String Matching
While the reconstruction process is designed to match the original string, it may not always produce an exact match. Deviations can occur due to factors such as repetitive sequences, sequencing errors, or ambiguities in the k-mers. The limitations of the De Bruijn graph approach may lead to variations between the reconstructed string and the original one.

Feel free to explore and adapt this code for your specific needs. The provided implementation offers a basic yet informative exploration of k-mer composition and string reconstruction techniques.






