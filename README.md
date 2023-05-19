# 香菜Bot

香菜Bot--基于chatgpt与stable diffusion和go-cqhttp的QQ机器人


>闲来无事，利用chatgpt的api和stable_diffusion的api写了一个qq机器人，qq使用的框架是go-cqhttp.这里做一些总结.
>赛博(女)朋友

项目结构：
qqchat_v0.2 
   >--chat
   >
   >-----chat.py
   >   
   >-----favicon.ico
   >   
   >-----requirements.txt
   >   
   >--go-cqhttp
   >
   >-----省略
   >   
   >--stable-diffusion-webui
   >
   >-----省略
   >   

对于以上项目结构，仅提供chat文件夹内内容，和其余两个开源项目所需要的一些内容

## 效果图
>废话不多说，先看看效果

![6V_QT~95`8G5EFG3(KPT}YK](https://github.com/Cc-Love-Study/XiangCaiBot/assets/92032190/1dd92891-5ff9-4ad7-81cd-1840913e1e90)

## 需要组件
	1. stable diffusion
	https://github.com/AUTOMATIC1111/stable-diffusion-webui
	2. go-cqhttp
	https://github.com/Mrs4s/go-cqhttp


## 配置方法
	1.对于stable diffusion 这里使用的是下面这个模型
	https://civitai.com/models/24779/dark-sushi-mix-mix
	2.如果希望每次自定义形象，可以使用梦作家 下面这个插件训练自己的模型
	https://github.com/7eu7d7/DreamArtist-sd-webui-extension
	如果使用默认形象，将
	xiangcai_embedding-5000.pt 和 xiangcai_embedding-5000-neg.pt放入
	stable-diffusion-webui/embedding内
	3.对于chat.py
	需要配置自己的chatgpt的key 因为要使用gpt的接口，所以电脑需要挂着魔法
	还有port需要和go-cqhttp内设定的一样 我这里使用的是9991
	同时 程序内的所有路径，都需要更改，因为我使用的是绝对路径，这里需要改为你自己的对应位置的路径
	4.对于go-cqhttp
	配置自己的qq信息就可以了 需要注意的是需要将表情包放入data/images内 表情包位置：
	链接：https://pan.baidu.com/s/15ORgOTm5icL2Av2aTdLnrw?pwd=1111 
	提取码：1111  下载img文件夹内容 放入data/images内部 可根据自己喜好添加表情包

![image](https://img2023.cnblogs.com/blog/2729131/202305/2729131-20230519205750040-1446506287.png)

![image](https://img2023.cnblogs.com/blog/2729131/202305/2729131-20230519205817046-2044091758.png)

![image](https://img2023.cnblogs.com/blog/2729131/202305/2729131-20230519205837581-406794619.png)

![image](https://img2023.cnblogs.com/blog/2729131/202305/2729131-20230519205847059-634959057.png)

![image](https://img2023.cnblogs.com/blog/2729131/202305/2729131-20230519205913034-263158540.png)

## 启动方法
	1.运行stable diffusion 这个启动比较慢 可能要等一会
	2.运行go-cqhttp 这个需要配置一些东西，可以看go-cqhttp的教程
	3.运行chat.py

## 项目环境
	见 
	requirement.txt
