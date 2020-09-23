# vcahin 阅读笔记

## 阅读过程
    
### 过程记录

**0. Abstract:**  
    首先调研基于数据库的可验证查询过程的处理问题. In this paper, we take thefirst step toward investigating the problem of verifiable queryprocessing over blockchain databases.   
    作者提出了一个基于累加的权限认证数据结构,该数据结构允许基于任意查询属性的动态聚合;为了更高效的查询验证, 两个新的索引被进一步开发来完成区块内部和区块外部的数据记录聚合.   
    作者还提出了倒转前缀树的结构来加速大量的订阅查询数据的并行处理速度

**1. Introduction**  
    有需求,先前的工作主要还是基于可信第三方来执行查询操作;  完整性验证
    对于轻节点来说将查询交给全节点来做, 情节点接受结果即可; 一个重要的事情在于验证结果的完整性
    做法: 每个区块中新增授权数据结构--->构建加密证明--->验证 验证物体(verification object)
    
**2. REALTED WORK**  
    验证数据结构ADS authenticated data structure和可验证的物体VO verifiable object的提出有赖于先前的工作

**3. PROBLEM DEFINITION**  
    最终的问题导向设计合理的ADS方法和简要介绍了时间窗口查询和订阅查询的工作方式

**4. PRELIMINARIES**  
    哈希函数
    双线性配对
    密码学超集累加器

**5. BAISC SOLUTION**  
主要方法介绍

**6. BATCH VERIFICATION**  
验证时间范围方法

**7. VERIFIABLE SUBSCRIPTION QUERIES** 
验证订阅方法

**8. SECURITY ANALYSIS**  
安全分析

**9. PERFORMANCE EVALUATION**  
性能分析

**10. CONCOLUSION**  
结论
	
## 扩展知识

### 布尔查询
使用and\or\not等逻辑运算符连接器俩的数据库查询算法(最简单的是线性)
### 双线性配对
双线性映射定义了三个素数$p$阶群乘法循环群$G_1,G_2和G_T$。
并且定义在这三个群上的一个映射关系$e:G_1*G_2{\rightarrow}G_T$，并且满足以下的性质：
1. 双线性：对于任意的$g_1{\in}G_1,g_2{\in}G_2,a,b{\in}Z_p$，均有$e(g_1^a,g_2^b)=e(g_1,g_2)^{ab}$成立；
2. 非退化性：满足${\exists}g_1{\in}G_1,g_2{\in}G_2满足e(g_1,g_2){\not ={1_{G_T}}}$。
3. 可计算性：存在有效的算法，对于${\forall}g_1{\in}G_1,g_2{\in}G_2$，均可计算$e(g_1,g_2)$。

如果$G_1=G_2$则称上述双线性配对是对称的，否则是非对称的。
另外，上述的双线性配对是素数阶的，还存在一种合数阶的双线性配对，最早也是由Boneh等人在[3]中引入密码学领域的。
合数阶双线性配对利用子群的正交性可以在实现更加复杂的功能前提下完成安全性证明。
### 加密重集累加器
acc以防碰撞方式将多集映射到某个循环乘法组中的某个元素


## 读后感悟
	隐私保护,加速处理
