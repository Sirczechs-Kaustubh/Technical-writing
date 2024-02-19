# How to align sequences like a pro : Global vs Local Alignments

Sequence alignment is a fundamental technique in bioinformatics, offering valuable insights into the evolutionary relationships, functions, and structures of biological entities.

In essence, sequence alignment involves comparing two sequences (known as pairwise alignment) or multiple sequences. This comparison is achieved by identifying a series of individual characters or patterns that appear in the same order across the sequences. The aim is to align these sequences in a way that highlights their similarities.

To elaborate, imagine you have two strings of letters, and you want to see how similar they are. You could line them up and look for places where the same letter appears in both strings. That’s the basic idea behind sequence alignment.

In the context of bioinformatics, these “strings” are usually sequences of DNA, RNA, or protein. By aligning these sequences, scientists can learn a lot about how different organisms are related (evolutionary relationships), what certain genes do, and how proteins fold into different structures.

Remember, sequence alignment is more than just a matching game. It’s a tool that helps us understand the very blueprint of life.

## Local Alignment 
***Local Alignment*** is a method that identifies regions of similarity within long sequences that are often widely divergent overall. It is used when the sequences to be aligned contain regions of similarity within their larger sequence, such as genes within genomes or domains within proteins.

### Analogy   
***Local alignment*** is like trying to find the most similar patches of fabric in two quilts of different sizes and patterns. You don’t have to align the whole quilts, just the parts that are most similar. You can also ignore the gaps or spaces between the patches, because they don’t affect the similarity score. The goal is to find the alignment that maximizes the similarity score and the number of matching patches
Example -


## Global alignment 
***Global Alignment*** attempts to align every residue in every sequence. It is most useful when the sequences in the query set are similar and of roughly equal size. This type of alignment considers all possible alignments and gap placements and chooses the best alignment that maximizes the match and minimizes the gaps.

### Analogy 
***Global alignment*** is like trying to match two strings of beads of different lengths and colors. You have to align them from end to end, and you can insert gaps or spaces between the beads to make them fit better. However, you have to pay a penalty for each gap you introduce, because it means that the beads are not perfectly matched. The goal is to find the alignment that minimizes the total penalty and maximizes the number of matching beads.

<img width="691" alt="image" src="https://github.com/PetBiotech/Technical-Writing/assets/116794066/984c2e54-517e-46d1-99e3-3d10deb1aff9">


| Differences | Local Alignment | Global Alignment |
| ----------- | --------------- | ---------------- |
| Definition | In local alignment, an attempt is made to find local regions with the highest level of similarity between the two sequences. | In global alignment, an attempt is made to align the entire sequence (end to end alignment). |
| Alignment | Here a substring of the query sequence is aligned to a substring of a target sequence. | Here all the characters from both query and target sequences are aligned. |
| Suitability | Any two sequences can be locally aligned as local alignment finds stretches of sequences with high level of matches without considering the alignment of rest of the sequence regions. | If two sequences have approximately the same length and are quite similar, they are suitable for global alignment. |
| Usage | Suitable for aligning more divergent sequences or distantly related sequences. | Suitable for aligning two closely related sequences. |
| Application | Used for finding out conserved patterns in DNA sequences or conserved domains or motifs in two proteins. | Used for comparing homologous genes like comparing two genes with same function (in humans vs mouse) or comparing two proteins with similar functions. |


## Conclusion
In this article, you have learned the difference between global and local alignment, and how to choose the best method for your analysis. Global alignment is useful for comparing sequences that are similar in length and have a high degree of similarity throughout. Local alignment is useful for finding regions of high similarity within long or dissimilar sequences. Both methods have their advantages and disadvantages, and you should consider the nature and purpose of your comparison before applying them.
