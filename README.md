# DZM_happiness_dinning
# 段志敏大作业_阿里天池幸福感挖掘
本次大作业，我们参加的是阿里天池的幸福感挖掘竞赛，下面简要介绍

## 使用模块
使用了如下模块  
**pandas**  
**matplotlib**  
**seborn**  
**numpy**  
**scipy**  
**sklearn**  
**warnings**  
**datetime**  
**catboost**  
**xgboost**  

## 编译环境
语言：python  3.x  
运行环境：jupyter notebook
## 使用说明

在安装jupyter notebook之后  
- 导入数据  
**happiness_submit**  
**happiness_test_abbr**  
**happiness_test_complete**  
**happiness_train_abbr**  
**happiness_train_complete**  
- 导入代码  
**happiness.ipynb**  
在确认函数包均安装到位后即可运行

## 代码结构说明
**cat_result**存储的是CatBoostRegressor模型的结果  
**xg_result**存储的是xgboost模型的结果  
**gbd_result**存储的是gbdt模型的求解结果   
**lr_result**存储的是带权平均融合CatBoostRegressor + xgboost + gbdt模型的结果  
**happiness_submit**是提交的结果  
**happiness_test_abbr**是精简的测试数据  
**happiness_test_complete**是完整的测试数据   
**happiness_train_abbr**是精简的训练数据  
**happiness_train_complete**是完整的训练数据  
**happiness_index**index文件中包含每个变量对应的问卷题目，以及变量取值的含义  
**total**是中间的数据处理结果  

## 目录结构
.
│  happiness_submit.csv  
│  happiness_test_abbr.csv  
│  happiness_test_complete.csv  
│  happiness_train_abbr.csv  
│  happiness_train_complete.csv  
│  happine_prediction.ipynb  
│  list.txt  
│  total.csv  
│  
├─.ipynb_checkpoints  
│      loglap-checkpoint.ipynb  
│      logmh-checkpoint.ipynb  
│      
├─cat_result  
│      cat0  
│      cat1  
│      cat10  
│      cat11  
│      cat12  
│      cat13  
│      cat14  
│      cat2  
│      cat3  
│      cat4  
│      cat5  
│      cat6  
│      cat7  
│      cat8  
│      cat9  
│      
├─gbd_result    
│      gbdt0  
│      gbdt1  
│      gbdt10  
│      gbdt11  
│      gbdt12  
│      gbdt13  
│      gbdt14  
│      gbdt2  
│      gbdt3  
│      gbdt4  
│      gbdt5  
│      gbdt6  
│      gbdt7  
│      gbdt8  
│      gbdt9  
│      
├─lr_result   
│      lr0  
│      lr1  
│      lr10  
│      lr11  
│      lr12  
│      lr13  
│      lr14  
│      lr2  
│      lr3  
│      lr4  
│      lr5  
│      lr6  
│      lr7  
│      lr8  
│      lr9  
│      
└─xg_result  
        xg0  
        xg1  
        xg10  
        xg11  
        xg12  
        xg13  
        xg14  
        xg2  
        xg3  
        xg4  
        xg5  
        xg6  
        xg7  
        xg8  
        xg9  
        



## 训练模型
采用了CatBoostRegressor模型、xgboost模型、gbdt模型三个模型进行求解  
最后采用了三个模型结果的带权平均值作为最终结果  






