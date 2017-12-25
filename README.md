## 情感分析的神经网络方法

### 复现过程：

前提：
* 使用邀请码在官网进行注册
* [在本地安装 cli 客户端](http://docs.russellcloud.com/get-started/install.html)
* 在cli客户端通过login登录

第一步：在官网创建项目
点击 项目创建页 创建项目，默认环境选：keras


第二步：绑定本地项目

```
#clone项目代码
git clone https://github.com/RussellCloud/Sentiment_Analysis.git

#进入项目目录
cd Sentiment_Analysis

#创建项目
russell init --name Sentiment_Analysis
```

第三步：训练模型

```
#运行模型训练代码并引用数据云上已经准备好的数据集
russell run --gpu --mode jupyter --data bad5f44ac4114d55939edf4f6bbe6dcb:data


#训练结束后通过info命令获取项目输出output_id
russell info <run_id>

#通过output命令在浏览器中查看或下载输出文件
russell output <run_id>

```



