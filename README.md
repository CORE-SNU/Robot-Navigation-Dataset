12, 9, 2024

# Robot Navigation [[Link](https://www.dropbox.com/scl/fo/jal4vuz9m607ltwnsplpo/ADAo3ByWRyhoYRhtjdnLrEE?rlkey=m370khijyrr7a0y70ozsj8dct&st=0eg0be8u&dl=0)]

A multi-modal dataset collected by a mobile robot in a crowded indoor environment. 

## Overview

The dataset consists of the following:
- point clouds measured by 32-channel Ouster OS1 LiDAR (measured in 10Hz)
- images received from Intel D435 RGBD camera (measured in 20Hz)
- odometry data (meausred in 50Hz)
The dataset will be consistently updated as we aim to collect diverse data under various domain shift scenarios.

## Datasets version

### Key Application

```mobile robot navigation```, ```dynamic obstacle avoidance```, ```etc```




### Dataset Characteristics
Each trajectory is 30 seconds long. Currently, there are 60 trajectories in our dataset.
-  Total number of images: 36,000
- Total number of pcd files: 18,000

### Labels

The included data are raw sensory inputs, thus having no labels. 
However, we are planning to add labels to existing data so that they can be used to train state-of-the-art perception models.

### Directory Structure

```
.
├── odometry
│   ├── trajectory1.csv
│   ├── trajectory2.csv
│   ├── ...
│   └── trajectory60.csv
└── pcds
│    ├── trajectory1
│    │   ├── 001.pcd
│    │   ├── 002.pcd
│    │   ├── ...
│    │   └── 300.pcd
│    ├── ...
│    └── trajectory60
└── images
       ├── trajectory1
       │   ├── 001.png
       │   ├── 002.png
       │   ├── ...
       │   └── 600.png
       ├── ...
       └── trajectory60
```

## Citing Datasets

If you use **this datasets** in your research, please use the following BibTeX entry.

``` bibtex
@misc{jaeukshin2024robot,
  author =       {Jaeuk Shin},
  title =        {Robot Navigation},
  howpublished = {\url{[http://github.com/hubtime-kmbae/CAML](https://github.com/CORE-SNU/Robot-Navigation-Dataset)}},
  year =         {2024}
}
```

---

Please email <sju5379@snu.ac.kr> to report any issues.
