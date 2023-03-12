# visual-chatgpt-colab
在colab上运行visual-chatgpt

https://colab.research.google.com/drive/1AyAG9lXHFZu4OHQ1taAcHL01sbZ9OcAb

# 手动替换的点
1、download.sh里没有必要下载模型，colab显存没那么大，下了也没法直接用，等低显存优化

2、对应地,visual-chatgpt里ConversationBot类也要注释掉一些不用的模型和Tools,以及修改cuda指定设备,,不然爆显存或者找不到卡,具体见代码第800行开始

3、export openaikey，windows和colab上都没有成功，直接修改visual-chatgpt.py了，第940行加入
>os.environ["OPENAI_API_KEY"] = "yourkey"

4、搞完后用gradio分享出公共链接，参数要加上share=True
>demo.launch(server_name="0.0.0.0", server_port=7860, share=True)

# 示例
![image](https://github.com/myrzx/visual-chatgpt-colab/blob/main/vis2.png)
