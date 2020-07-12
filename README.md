# Modularized Framework with Category-Sensitive Abnormal Filter for City Anomaly Detection (ACMMM Multimedia Grand Challenge 2020)

This repository contains source codes of team SYSU-BAIDU for CitySCENE Challenge 2020, and the technical details please refer to the paper
"Modularized Framework with Category-Sensitive Abnormal Filter for City Anomaly Detection". 

Our framework obtains a 66.41 MF1 in the test set of the CitySCENE Challenge 2020, which ranks first in the specific anomaly detection task. 

## Requirements

- MMdetection

- Pytorch >=1.1.0

- cuda9

- cudnn7.5


#### Docker for reproducing our results:

Please download the images in [link](https://drive.google.com/file/d/1zLqjvXYkHULTByK5XH-vRDa7jRpq-iSF/view?usp=sharing), then 
```
curl -L -o b53a0eea3f76  https://drive.google.com/file/d/1zLqjvXYkHULTByK5XH-vRDa7jRpq-iSF/view?usp=sharing
docker load b53a0eea3f76 
docker run --gpus all --network none -ti -v <testset_path>:/testset:ro  b53a0eea3f76 /bin/bash
bash /home/example.sh
cltr+d (exit)
docker cp aecd3ec1e4d4:result/task1 ./           
docker cp aecd3ec1e4d4:result/task2 ./
```
The code is released in the docker.

#### If you have any questions or issues in using this code, please feel free to
contact us (wujie10558@gmail.com)
