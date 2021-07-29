# FVD based on ViT
https://gitee.com/h-Sun/FVD-based-on-ViT
#### 介绍
使用ViT模型提取图像特征计算FVD值

#### 结构说明
    FVD:
        代码文件：
            vitdefined_5.py          (ViT的网络结构定义，主要完成进行图像特征提取)
            ViT_5.py   	             (处理输入的文件类型，获取图像并将帧数维度拼接到图片宽，调用vitdefined_5.py返回特征)
            fvd.py           		 (计算fvd的值)
            example.py       		 (随机生成两组activation进行fvd模块调用及FVD值计算的测试)
	        test_5.py				 (进行5帧紫外源图像FVD值的计算）
        文件夹：
            fvd_100valid            (100次random测试的箱形图)
            Generator_Out           (1000张生成的图片，由于大小限制只上传了100张)
            type        			(存放部分样本pickle文件)
            vit         			(存放vit模型)

#### 使用说明
python3 test_5.py
