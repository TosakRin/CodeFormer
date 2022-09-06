## issue

**Training Code**: This paper is under review now, thus, we plan to release the training code and other models once the paper is accepted(Aug 1)

**Task of Color image**: Currently, we have only released the model for face restoration, the models for color enhancement and inpainting are not released yet



## code 实现细节

`inference_codeformer.py` 

1. 设定入口参数

2. 处理输入输出路径

3. 设置 background upsampler

4. 设置 CodeFormer restorer

5. 设置 FaceRestoreHelper

   **开始正式处理**, 遍历每一张图片:

   ---

6. 人脸: resize

   全图: 检测人脸, align_warp_face

7. 遍历每一张人脸, 归一化到01之间, 进行face restore,  

8. 将对图像进行超分, 把人脸贴回去

9. 保存所有图像

## 结论

1. 训练集似乎使用的是白人数据集, 人脸有明显的白人特征 
2. 论文还未发表, 没有训练代码
