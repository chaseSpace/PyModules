## 这是一个调用时间的模块，我根据自己的习惯重新封装了`time`，你可以试试~

### 包含以下time自带的方法  
----
* strptime  
* strftime  
* localtime  
* ctime  
* sleep  
* clock  

### 下面是我新增的方法
----
* timestamp ：轻松获取各类时间戳  
秒级时间戳：  
```
print niceTime.timestamp()  #1523717093
```
原始时间戳：  
```
print niceTime.timestamp(0) #1523717093.6
```
毫秒级时间戳： 
```
print niceTime.timestamp(13) #1523717093599
```

* now_time_elements ：可传入时间戳获取对应的时间，以列表格式返回
```
timestamp = niceTime.timestamp()  
print niceTime.now_time_elements(timestamp) #[2018, 4, 14, 18, 19, 1, 5, 104, 0]
```