# A-New-Fast-and-Accurate-Heuristic-for-the-Automatic-Scene-Detection-Problem


This is the repository for the paper "A New Fast and Accurate Heuristic for the Automatic Scene Detection Problem", by D. Catanzaro, R. Pesenti, and R. Ronco.<br>

<h1>Dataset files</h1>
According to the notation used in Section 4 of the paper, the folder <i>I1</i> contains the distance matrices related to the instances solvable with Heuristic-Partitioner, Rotman-T, Rotman-H, and Additive-Heuristic-Partitioner while the folder <i>I2</i> contains the data of the instances only solvable with Heuristic-Partitioner and Additive-Heuristic-Partitioner (on our 24GB RAM hardware).
<br>

<!-- Each instance *i* is associated with the two files *i.npy* and *i.txt*: the former contains the numpy encoding of the distance matrix associated to the video *i*, while the latter contains the ground-truth partition of *i*. Specifically, *i.txt* reports the last shot of each scene in the ground-truth partition in increasing order. -->


<h1>Implementation files</h1>

The folder *src* contains the python sources needed to run the algorithms. For instance, in order to solve the ASDP on Big Buck Bunny encoded as the numpy distance matrix in the file *Big_Buck_Bunny.npy* for a number of scenes K = 20 by using Heuristic-Partitioner, run:<br>

python asdp_solver.py Big_Buck_Bunny.npy 20 Heuristic-Partitioner

In order to solve the same instance with Rotman-T, Rotman-H or Additive-Heuristic-Partitioner, please replace *Heuristic-Partitioner* with *Rotman-T*, *Rotman-H*, or *Additive-Heuristic-Partitioner*, respectively.
