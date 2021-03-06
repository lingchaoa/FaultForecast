## 风机叶片开裂故障预警 
### 任务描述
SCADA是风场设备管理、监测、和控制的重要系统，通过实时收集风机运行的环境参数、工况参数、状态参数和控制参数使风场管理者能够实时了解风电装备资产的运行和健康状态。基于SCADA数据建立叶片开裂模型，对早期叶片开裂故障进行告警，可以避免风场因叶片开裂导致的更大损失，提升风机运行稳定性，提升机组发电量。  
参赛选手要基于风机SCADA实时数据，通过机器学习、深度学习、统计分析等方法建立叶片开裂早期**故障检测模型**，对叶片开裂故障进行提前告警。

### 数据说明
train: 本文件中存放用于训练的采集数据，每个CSV为10分钟内采样得到的一个样本点。  
test: 本文件中存放用于测试的采集数据，每个CSV为10分钟内采样得到的一个样本点。  
train_labels.csv 用户训练的标注信息。  
内容格式如下：


|ID|Label|
:----|:----|
XXXXXX | 0 
XXXXXY | 1  

注：ID为csv样本文件名称，Label为本文件对应的标注信息，0表示该样本点对应风机一周内未发生故障，1表示该样本点对应的风机在一周内发生故障。  
### 评分标准
![image-20210817112845274](https://bigdata66.oss-cn-shanghai.aliyuncs.com/img/image-20210817112845274.png)
[比赛地址](https://www.datafountain.cn/competitions/302/details)
