
# video2bvh2.0
https://github.com/Dene33/video_to_bvh but with python 3 and tensorflow2.0

Uses [Openpose](https://github.com/CMU-Perceptual-Computing-Lab/openpose) to crop frames around a single person and then uses [hmr2.0](https://github.com/russoale/hmr2.0) by [Russoale](https://github.com/russoale) to get 3D pose keypoints. Then, using [Dene33](https://github.com/Dene33/)'s fork of [hmr](https://github.com/Dene33/hmr), the 3D pose keypoints are converted to bvh.

![Demo gif](media/rough_demo.gif)

Input video is [Man dancing on rooftop](https://www.pexels.com/video/man-dancing-on-rooftop-2795750/) by [cottonbro](https://www.pexels.com/@cottonbro). The bvh on the left is lagging slightly behind the video on the right. Will upload better demo videos later.

To Do:

 - [ ] Apply filters to smoothen the wobblyness
 - [ ] Add support for multiple videos at once
 - [ ] If I get time, Dash inline application.

**References:**

[Dene33's video to bvh](https://github.com/Dene33/video_to_bvh)  
[hmr by akanazawa](https://github.com/akanazawa/hmr)  
[Russoale's hmr2.0](https://github.com/russoale/hmr2.0)  
[Openpose](https://github.com/CMU-Perceptual-Computing-Lab/openpose)  
[Openpose Colab notebook by tugstugi](https://colab.research.google.com/github/tugstugi/dl-colab-notebooks/blob/master/notebooks/OpenPose.ipynb)  
[Dene33's fork of hmr](https://github.com/Dene33/hmr) 

**hmr citation:**
```
@inProceedings{kanazawaHMR18,
  title={End-to-end Recovery of Human Shape and Pose},
  author = {Angjoo Kanazawa
  and Michael J. Black
  and David W. Jacobs
  and Jitendra Malik},
  booktitle={Computer Vision and Pattern Recognition (CVPR)},
  year={2018}
}
```
**Openpose citations:**
``````
@article{8765346,
  author = {Z. {Cao} and G. {Hidalgo Martinez} and T. {Simon} and S. {Wei} and Y. A. {Sheikh}},
  journal = {IEEE Transactions on Pattern Analysis and Machine Intelligence},
  title = {OpenPose: Realtime Multi-Person 2D Pose Estimation using Part Affinity Fields},
  year = {2019}
}

@inproceedings{simon2017hand,
  author = {Tomas Simon and Hanbyul Joo and Iain Matthews and Yaser Sheikh},
  booktitle = {CVPR},
  title = {Hand Keypoint Detection in Single Images using Multiview Bootstrapping},
  year = {2017}
}

@inproceedings{cao2017realtime,
  author = {Zhe Cao and Tomas Simon and Shih-En Wei and Yaser Sheikh},
  booktitle = {CVPR},
  title = {Realtime Multi-Person 2D Pose Estimation using Part Affinity Fields},
  year = {2017}
}

@inproceedings{wei2016cpm,
  author = {Shih-En Wei and Varun Ramakrishna and Takeo Kanade and Yaser Sheikh},
  booktitle = {CVPR},
  title = {Convolutional pose machines},
  year = {2016}
}
``````
