# Spark

> 观看Spark公开课记录

1. 主从结构，职责
   1. 接受客户端请求（任务）
   2. 资源的管理和任务的分配
   3. 部署方式（Standalone、Yarn、Mesos（资源管理容器）、k8）
   4. 主节点Cluster Manager ，Worker是节点上的资源和任务的管理者。一个worker可以启动多个（executor）
2. 启动方式：
   1. 工具spark-submit（提交任务）
   2. 工具spark-shell（命令行）
   3. 核心方法：main方法（创建一个核心对象，SparkContext）通过SparkContext连接到Master上提交任务。
      1. 提交任务请求给master
      2. 分配资源
      3. 直接提交任务给master执行

