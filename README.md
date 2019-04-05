# Our 2D-Assisted Self-supervised Learning (2DASL) is available at: https://arxiv.org/abs/1903.09359 

[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/joint-3d-face-reconstruction-and-dense-face/face-alignment-aflw2000-3d)](https://paperswithcode.com/sota/face-alignment-aflw2000-3d?p=joint-3d-face-reconstruction-and-dense-face)

This project is created by Tu Xiaoguang (xguangtu@outlook.com) and Luo Yao (luoyao_alpha@outlook.com). Any questions pls open issues for our project, we will reply quickly. 

To facility the research in the community of 3D face reconstruction and 3D face alignment, we release our source code, including the pytorch code for testing (training code will be available upon the acceptance of our paper), the matlab code for 3D plot, 3D face rendering and evaluation. 

Landmark detection (only 68 landmarks are plotted to show)

![lmks_res](https://user-images.githubusercontent.com/8948023/55403032-76960580-5587-11e9-926b-4be4d72c3e3f.gif)

3D face reconstruction 

![3df_res](https://user-images.githubusercontent.com/8948023/55403128-b3fa9300-5587-11e9-92f0-b7733431ddc9.gif)

Dense face alignment

![dense_res](https://user-images.githubusercontent.com/8948023/55403191-e0161400-5587-11e9-8633-89c8681cf7ed.gif)


# We add the matlab evaluation code with the metric Normalized Mean Error (NME) in the folder "evaluation", including:
  1. We compare the results of our 2DASL with PRNet on the sparse 68 key points on both 2D&3D coordinates.  
  2. We compare the results of our 2DASL with 3DDFA on all points for the task of dense alignment (both 2D and 3D coordinates) and
     3D face recnostruction.
  3. The Iterative Closest Point (ICP) algorithm, which is used to find the nearest points between two 3D models is included in our code.
     
  Usage: Download the "visualize.rar" package at： https://pan.baidu.com/s/1M0sg3eqrtzxxMJqmAzczRw using the password: "h26t".
         Putting the package under the folder "evaluation", extracting it and then run the scripts: "nme_for_*". 
         
# We add our test code in the folders "models" and "test_codes", including:
  1. The 2DASL models for stage1 and stage2, in the folder "models".
  2. The test code to obtain 3D vertex for ALFW2000-3D images.
  3. The code to plot 2D facial landmarks.
  
  Usage: python-3.6.6, pytorch-0.4.1. Just run the script "main_visualize_plot_4chls.py" in the folder "test_codes".
  
# We add our 3D face rendering code in the folder "3D_results_plot", including:
  1. The code for 3D face rendering, i.e., drawing 3d reconstruction mask.
  2. The code for plotting dense face alignment.
  3. The code for writing .obj file, the .obj files could be opend by the software meshlab. 
  
  Usage: Download the "visualize.rar" package at： https://pan.baidu.com/s/1M0sg3eqrtzxxMJqmAzczRw using the password: "h26t".
         Putting the package under the folder "3D_results_plot", extracting it and then run the script "test_good_byXgtu.m". 
                  
# Acknowledgement
Thanks for the authors of [3DDFA](https://github.com/cleardusk/3DDFA) and [PRNet](https://github.com/YadiraF/PRNet) for making their excellent works publicly available.

# Additional example 
![xgtu-lmks_res](https://user-images.githubusercontent.com/8948023/55405030-cb3b7f80-558b-11e9-9553-e1858db0e198.gif) 

 # Citation
  If you find our code is useful for your research, pls cite our work:
```  
@article{tu2019joint,
  title={Joint 3D Face Reconstruction and Dense Face Alignment from A Single Image with 2D-Assisted Self-Supervised Learning},
  author={Tu, Xiaoguang and Zhao, Jian and Jiang, Zihang and Luo, Yao and Xie, Mei and Zhao, Yang and He, Linxiao and Ma, Zheng and Feng, Jiashi},
  journal={arXiv preprint arXiv:1903.09359},
  year={2019}
}
```



