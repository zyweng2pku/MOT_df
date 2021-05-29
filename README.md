# MOT_df
Real-Time Multiple Object Tracking with Discriminative Features, accepted by ICARCV 2020.

## Overview ##
This method is real-time multiple object tracking based on [FairMOT](https://github.com/ifzhang/FairMOT/)[1]. Different from FairMOT, we mainly explore the association stage by using new association strategy and online learning method to learn effective features.

## Building ##
Requisites: python

Clone the FairMOT project and replace the multitracker.py file and the matching.py file in the src/lib/tracker dir.

After that, run the demo according to the instructions in [FairMOT](https://github.com/ifzhang/FairMOT/)


## Result Update ##
It should be noted that in the ICARCV paper, we use the FairMOT_v1 network. Now, since the network is optimized, which is called FairMOT_v2 in the recent MOT papers, we apply our method on FairMOT_v2, and it still works. The updated results on MOT16 training dataset are below.
| Method  | IDF1 | MOTA | IDs |
| ------- | ---- | ---- | ---- |
| FairMOT_v2  | 81.9% | 83.3% | 544 |
| ours  | 82.3%  | 83.3% | 514 |
 


## Reference ##
[1] Zhang, Yifu, Chunyu Wang, Xinggang Wang, Wenjun Zeng, and Wenyu Liu. "FairMOT: On the Fairness of Detection and Re-Identification in Multiple Object Tracking." arXiv preprint arXiv:2004.01888 (2020).



Please cite:
```
@inproceedings{WengZLL20,
  author    = {Zhenyu Weng and
               Yuesheng Zhu and
               Zhiping Lin and
               Haizhou Li},
  title     = {Real-Time Multiple Object Tracking with Discriminative Features},
  booktitle = {16th International Conference on Control, Automation, Robotics and
               Vision, {ICARCV} 2020, Shenzhen, China, December 13-15, 2020},
  pages     = {309--314},
  publisher = {{IEEE}},
  year      = {2020},
}
```

## Acknowledgement ##
This work is based on FairMOT(https://github.com/ifzhang/FairMOT/). Thanks for their wonderful works.


