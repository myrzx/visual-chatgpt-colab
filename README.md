# 原项目地址
https://github.com/microsoft/visual-chatgpt

# visual-chatgpt-colab
在colab上运行visual-chatgpt

https://colab.research.google.com/drive/1AyAG9lXHFZu4OHQ1taAcHL01sbZ9OcAb

# 使用方法
1、%env OPENAI_API_KEY={'yourkey'}中，把yourkey替换成自己的API key

2、想尝试其他模型，原项目GPU memory usage里有模型名字，在启动参数load里以模型名_cuda:GPU号格式添加，示例如下
>"ImageCaptioning_cuda:0,Text2Image_cuda:0,Image2Canny_cuda:0"

>官方colab参数：
"Text2Image_cuda:0,ImageCaptioning_cuda:0,VisualQuestionAnswering_cuda:0,Image2Canny_cpu,Image2Line_cpu,Image2Pose_cpu,Image2Depth_cpu,CannyText2Image_cuda:0,InstructPix2Pix_cuda:0,Image2Seg_cuda:0"

# 示例
![image](https://github.com/myrzx/visual-chatgpt-colab/blob/main/vis2.png)
