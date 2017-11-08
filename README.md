Video eye-tracking database
==========
The video eye-tracking database containing the fixation data of 33 standard video sequences of HEVC, established by Lai Jiang, Mai Xu, Xin Deng in Beihang University(2015). 

The detail of this database as well as some observations are introduced in paper 'Learning to Detect Video Saliency With HEVC Features' ([link](http://ieeexplore.ieee.org/abstract/document/7742914/)).

## Usage
All fixation data are recorded in **'video_database.mat'**, where you can find

* videos_info: the information of 33 videos 

* video_names_list: the index for 33 videos

* subj_info: the information of 32 participants 

* subj_names_list: the index for 32 participants

* fixdata: contains fixation data of all videos from all participants, each row refers to a single fixation.

* fixdata_fields: 
    '1: SubjectIndex (see subj_names_list)'
    '2: VideoIndex (see video_names_list)'
    '3: Timestamp (milliseconds after image display)'
    '4: GazeDuration'
    '5-6: fixation position (take upper-lift corner as origin )'
   
e.g. If a row in fixdata is '6 29 4084 183 467 319', that means this fixation is in 'ChinaSpeed.avi' recorded from JL. The start time and the duration of this fixation is 4084ms and 183ms, respectively, with the location (467,391).

As a test, you can run **'demo.m'** to view the heatmaps of the target video.  

## Citation
One could freely use this database, if that, please cite with the following Bibtex code:
```
@article{xu2017learning,
  title={Learning to detect video saliency with HEVC features},
  author={Xu, Mai and Jiang, Lai and Sun, Xiaoyan and Ye, Zhaoting and Wang, Zulin},
  journal={IEEE Transactions on Image Processing},
  volume={26},
  number={1},
  pages={369--385},
  year={2017},
  publisher={IEEE}
}
```

## Contact
Should you have any queries, please contact jianglai.china@buaa.edu.cn / jianglai.china@aliyun.com

Have fun!
