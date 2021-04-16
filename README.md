# faster-rcnn
这个项目主要用来是记录整个faster rcnn项目从数据准备、训练、单张图片检测、文件夹图片检测、以及画出虚警、漏检等文件的描述
## 1、整个文件结构      
├─input    用来进行最终可视化输出的文件   
│  ├─detection-results  目标检测网络预测每张照片的txt结果     
│  ├─ground-truth    真实每张图片目标的box信息    
│  ├─images-optional    存放真实图片的文件夹    
│  └─outputs
├─model_data    # 用于存放各种配置文件的文件夹    
├─nets    
│  └─__pycache__    
├─utils    
│  └─__pycache__    
├─VOCdevkit   用来存放数据集文件夹    
│  └─VOC2007    
│      ├─Annotations      用于存放文件xml文件   
│      ├─Annotations-train   
│      ├─ImageSets   
│      │  └─Main   用于存放train.tx, test.txt等文件   
│      ├─JPEGImages   用于存放训练数据集图片的文件
│      └─JPEGImages-train   
└─__pycache__   

## 2、数据的准备工作
首先数据集应该需要符合VOC格式的要求，一共要包括xml文件和图片文件，将xml文件放在Annotations文件夹下，将图片数据集放在JPEGImages中
* 1、生成train.txt, trainval.txt等文件,主要利用
* 
