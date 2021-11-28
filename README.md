# Model-Swap-Face_v2
&emsp;&emsp;这个项目是基于<a href='https://github.com/NVlabs/stylegan2'>stylegan2</a> <a href='https://github.com/eladrich/pixel2style2pixel'>pSp</a>制作的，比<a href='https://github.com/a312863063/Model-Swap-Face'>旧版本</a>在推理速度和图像质量上有一定提升。主要的功能是将虚拟模特进行环球不同区域的风格转换，目前转换器提供西欧模特、东亚模特和北非模特三种主流的风格样式，可帮我们实现生产资料零成本化以及广告制作的高效化；此外项目还提供了去位姿编码器以获得模特的正脸肖像。转换器的版权所有：<a href='http://www.seeprettyface.com'>www.seeprettyface.com</a>。<br /><br />

# 效果预览
<p align="center">
	<img src="https://github.com/a312863063/Model-Swap-Face_v2/blob/main/docs/model_stylization.jpg" alt="Sample">
</p>

# 使用方法
## 环境配置
&emsp;&emsp;参照<a href='https://github.com/eladrich/pixel2style2pixel'>pSp</a>文档进行环境配置。

## 下载模型
&emsp;&emsp;模型下载地址参见`pretrained_models`文件夹中的文档，包括的模型主要如下：<br />
&emsp;&emsp;encoder.pt -- 含位姿编码器
&emsp;&emsp;encoder_without_pos.pt -- 去位姿编码器
&emsp;&emsp;projector_EastAsian.pt -- 东亚模特投射器
&emsp;&emsp;projector_WestEuropean.pt -- 西欧模特投射器
&emsp;&emsp;projector_NorthAfrican.pt -- 北非模特投射器

## 运行代码
&emsp;&emsp;将图片放在input文件夹下，然后编辑scripts/inference.py，运行如下代码结果会保存在output文件夹下：<br />
&emsp;&emsp;```python scripts/inference.py```

## 了解更多
&emsp;&emsp;我周末的时候喜欢思考一些新的应用场景和模式，欢迎访问<a href='http://www.seeprettyface.com'>我的网站</a>了解更多。
