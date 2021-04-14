# A-New-Fast-and-Accurate-Heuristic-for-the-Automatic-Scene-Detection-Problem


This is the repository for the paper "A New Fast and Accurate Heuristic for the Automatic Scene Detection Problem", authored by D. Catanzaro, R. Pesenti, and R. Ronco.<br>

<h1>Dataset files</h1>
According to the notation used in Section 4, the folder "I1" contains the data relevant to the instances solvable with Heuristic-Partitioner, Rotman-T and Rotman-H, while the folder "I2" contains the data relevant to the instances only solvable with Heuristic-Partitioner (on our 24GB RAM hardware).<br>

Each instance *i* is associated with the two files *i.npy* and *i.txt*: the former contains the numpy encoding of the distance matrix associated to the video *i*, while the latter contains the ground-truth partition of *i*. Specifically, *i.txt* reports the last shot of each scene in the ground-truth partition.


<h1>Implementation files</h1>

The folder *src* contains the python sources needed to run the algorithms. For instance, in order to solve the ASDP on Big Buck Bunny encoded as the distance matrix *Big_Buck_Bunny.npy* with the ground-truth *Big_Buck_Bunny.txt* by using Heuristic-Partitioner, run:<br>

python asdp_solver.py Big_Buck_Bunny.npy Big_Buck_Bunny.txt Heuristic-Partitioner

In order to solve the same instance with Rotman-T and Rotman-H, please replace *Heuristic-Partitioner* with *Rotman-T* and *Rotman-H*, respectively.
