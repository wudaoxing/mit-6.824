# 简介
* 目标  
构建一个 MapReduce 系统。 （类似于 MapReduce 论文中的东西）
  * 实现一个调用 application Map 和 Reduce functions并处理读取和写入文件的work process；
  * 以及一个将任务分发给works并处理failed workers的coordinator process。 

# 开始
* 用Go实现
* 使用git获取initial labsoftware
```
git clone git://g.csail.mit.edu/6.824-golabs-2022 6.824
```
  * 在 src/main/mrsequential.go 中提供了一个简单的sequential mapreduce 实现。 
    * 它在一个进程中一次运行maps和reduces。 
  * 还提供了几个 MapReduce 应用程序：
    * mrapps/indexer.go：文本索引器。 
    * mrapps/wc.go：字数统计。可以使用如下命令运行：
    ```
    
    ```
    （注意：-race 启用 Go race detector。建议使用race detector开发和测试 6.824 lab code。）
  * 