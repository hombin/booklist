# Kubernetes 权威指南（读书笔记）

### 概览

#### Kubernetes 

1. 基于容器技术的分布式架构
2. 开放平台不局限于任何语言
3. Service
   1. 分布式集群架构的核心，一个Service对象拥有如下关键特征
   2. 拥有唯一指定的名称（比如mysql-server）
   3. 拥有一个虚拟IP（Cluster IP、Service IP或VIP）和端口号
   4. 能够提供某种远程服务能力。◎ 被映射到提供这种服务能力的一组容器应用上



#### 资源对象

1. Master
   1. Kubernetes API Server（kube-apiserver）：提供了HTTP Rest接口的关键服务进程，是Kubernetes里所有资源的增、删、改、查等操作的唯一入口，也是集群控制的入口进程。
   2. Kubernetes Controller Manager（kube-controller-manager）：Kubernetes里所有资源对象的自动化控制中心，可以将其理解为资源对象的 “大总管”。
   3. Kubernetes Scheduler（kube-scheduler）：负责资源调度（Pod调度）的进程，相当于公交公司的“调度室”。
   4. 另外，在Master上通常还需要部署etcd服务，因为Kubernetes里的所有资源对象的数据都被保存在etcd中。
2. Node
   1. kubelet：负责Pod对应的容器的创建、启停等任务，同时与Master密切协作，实现集群管理的基本功能。
   2. kube-proxy：实现Kubernetes Service的通信与负载均衡机制的重要组件。
   3. Docker Engine（docker）：Docker引擎，负责本机的容器创建和管理工作。
3. 



### 容器编排

1. Swarm
2. Mesos
3. Kubernetes



#### docker 管理

