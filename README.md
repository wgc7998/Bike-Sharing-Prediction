# Bike-Sharing-Prediction
LinearRegression / RidgeCV / Lasso

1、 任务描述:
  在Capital Bikeshare （美国Washington, D.C.的一个共享单车公司）提供的自行车数据上进行回归分析。训练数据为2011年的数据，要求预测2012年每天的 单车共享数量。

2、 原始数据集地址：http://archive.ics.uci.edu/ml/datasets/Bike+Sharing+Dataset 

  1) 文件说明：
     day.csv: 按天计的单车共享次数（本代码只使用该文件） 
     hour.csv: 按小时计的单车共享次数（无需理会） 
     readme：数据说明文件
            
  2) 字段说明：
    Instant记录号 
    Dteday：日期 
    Season：季节（1=春天、2=夏天、3=秋天、4=冬天） 
    yr：年份，(0: 2011, 1:2012) 
    mnth：月份( 1 to 12) 
    hr：小时 (0 to 23) （只在hour.csv有，作业忽略此字段） 
    holiday：是否是节假日 weekday：星期中的哪天，取值为0～6 
    workingday：是否工作日 1=工作日 （是否为工作日，1为工作日，0为非周末或节假日 
    weathersit：天气（1：晴天，多云 2：雾天，阴天 3：小雪，小雨 4：大雨，大雪，大雾） 
    temp：气温摄氏度 
    atemp：体感温度 
    hum：湿度 windspeed：风速 
    casual：非注册用户个数 
    registered：注册用户个数 
    cnt：给定日期（天）时间（每小时）总租车人数，响应变量y
    
casual、registered和cnt三个特征均为要预测的y，本代码只对cnt进行预测
