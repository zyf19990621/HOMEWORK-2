# 网络及分布式计算第二次作业

#### 2017302580018  刘佳媚

---

### 1、P3

##### 考虑一个应用程序以稳定的速率传输数据（例如，发送方每丘个时间单元产生一个N比特的数据单 元，其中：较小且固定）。另外，当这个应用程序启动时，它将连续运行相当长的一段时间。回答下 列问题，简要论证你的回答： 

##### a. 是分组交换网还是电路交换网更为适合这种应用？为什么？

##### b. 假定使用了分组交换网，并且该网中的所有流量都来自如上所述的这种应用程序。此外，假定该 应用程序数据传输速率的总和小于每条链路的各自容量。需要某种形式的拥塞控制吗？为什么？

  解：

​        a、电路交换网。因为该应用将以稳定的速率传输数据，且会连续运行相当长一段时间，采用电路交换网可以有效利用带宽，会更经济。

​        b、不需要。因为即使在最坏的情况下，所有应用程序同时通过一个网络链路进行传输，此时的数据传输速率总和仍小于每条链路的容量，不会发生拥塞。



------

### 2、P5

##### 回顾在1.4节中的车队的类比。假定传播速度为100km/h。

##### a.假定车队旅行150km：在一个收费站前面开始，通过第二个收费站，并且正好在第三个收费站后 面结束。其端到端时延是多少？ 

##### b.重复（a）,现在假定车队中有8辆汽车而不是10辆口。

  解：

​        a、由1.4节可知：收费站将整个车队推向公路所需要的 时间是 t1:（10辆车）/（5辆车/min) = 2min;

​              旅行150km所需时间是 t2 : （150km） / （100km/h） = 1.5h;

​              总时间：t = 3 * t1 + t2 = 96min 。

​        b、收费站将整个车队推向公路所需要的 时间是 t1:（8辆车）/（5辆车/min) = 1.6min;

​              旅行150km所需时间是 t2 : （150km） / （100km/h） = 1.5h;

​              总时间：t = 3 * t1 + t2 = 94.8min 。

   

---

### 3、P13

##### a.假定有N个分组同时到达一条当前没有分组传输或排队的链路。每个分组长为厶，链路传输速率 为R。对N个分组而言.其平均排队时延是多少？ 

##### b.现在假定每隔LN/R秒有N个分组同时到达链路。一个分组的平均排队时延是多少？ 

  解：

​        a、第一个分组排队时延：0 ；第二个分组排队时延：L/R ；第三个分组排队时延：2L/R ；

​              依此类推得第N个分组排队时延：（N - 1）L/R 。

​              平均排队时延：（0 + L/R + 2L/R + ... +（N - 1）L/R）/ N = （N - 1）L/2R 。

​       b、因为第N个分组排队时延是（N - 1）L/R，所以当下一批 N 个分组到达时，上一批刚好已经传完。因此平均排队时延仍为 (N-1)L/2R 。