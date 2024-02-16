# Macrogenome-Sequence-Classification-Project

1. We use kth order Markov Chain to solve sequence prediction problem in bioinformatics

+ `genomes` contains ten reference genomes
+ `test.fa` contains several labeled sequence which can be used for model training or validation. The annotation file is `seq_id.map`
+ `reads.fa` is the unlabeled short sequences used for prediction

2.  In addition, the performance of GPU is further considered. 

- Applied `Python Numba` for `CUDA` Programming to realize GPU accelerate
- open 256 × 512 threads with grid step technology



Finally increased the accuracy from about 60% to 98.6% (9-th Markov Chain), reduced about 67.5% time with GPU.
