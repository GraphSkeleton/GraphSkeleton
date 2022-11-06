## Graph-Skeleton

This anonymous repository is for a code demo on dataset DGraph in  "Graph-Skeleton: 10% Node is Sufficient to Represent Massive Graph Data" (WWW 23')



### Install

Install libboost

```shell
sudo apt-get install libboost-all-dev
```

### Compile

Compile Graph-Skeleton

```shell
mkdir build
cd build
cmake ..
make
cd ..
```

### Data Download

The currently code demo is based on the dataset [DGraph](https://dgraph.xinye.com/dataset). Please unizp the dataset folder and organize as follows:
```
.
--DGraphFin
   └─dgraphfin.npz
```

### GraphS-Skeleton Generation
To generate skeleton graphs, a graph compressio script is provided. Please note that in our original paper, hyper-parameters "d1", "d2" are set as 2 and 1, you can also modify the setting of "d" in the script to change the node fetching distance.

```
python xinye_compression.py
```







