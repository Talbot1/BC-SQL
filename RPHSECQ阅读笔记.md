# Result Pattern Hiding Searchable Encryption for Conjucntion Search
为联合查询打造的结果模式隐藏的搜索加密

## 阅读过程

### 过程记录

**ABSTRACT**
不经意交叉标签 OXT (Oblivious Cross-Tags)协议 在查询对称加密 SSE searchable symmetric encryption 有重大的落地应用
基于OXT提出了隐藏交叉标签 HXT (Hidden cross-Tags)协议;移除了OXT中的关键词配对结果模式KPRP Keyword Pair Result Pattern的泄露
采用隐藏向量加密HVE (Hidden Vector Encryption) 和 概率索引(布隆过滤器) 的方式来实现关键词对结果模式的泄露

**INTRODUCTION**
介绍了OXT的工作原理和HXT使用的技术


**PRELIMINARIES**
符号表、TSet构建方法、布隆过滤器

**LIGHTWEIGHT SYMMETRIC-KEY HIDDEN VECTOR ENCRYPTION**
轻量对称密钥隐藏向量加密
没整明白

**HXT CONSTRUCTION**

**SECURITY**

**PERFORMANCE COMPARISON**
lt Pattern Hiding Searchable Encryption for Conjucntion Search
为联合查询打造的结果模式隐藏的搜索加密

## 阅读过程

### 过程记录

**ABSTRACT**
不经意交叉标签 OXT (Oblivious Cross-Tags)协议 在查询对称加密 SSE searchable symmetric encryption 有重大的落地应用
基于OXT提出了隐藏交叉标签 HXT (Hidden cross-Tags)协议;移除了OXT中的关键词配对结果模式KPRP Keyword Pair Result Pattern的泄露
采用隐藏向量加密HVE (Hidden Vector Encryption) 和 概率索引(布隆过滤器) 的方式来实现关键词对结果模式的泄露

**INTRODUCTION**
介绍了OXT的工作原理和HXT使用的技术


**PRELIMINARIES**
符号表、TSet构建方法、布隆过滤器

**LIGHTWEIGHT SYMMETRIC-KEY HIDDEN VECTOR ENCRYPTION**
轻量对称密钥隐藏向量加密
没整明白

**HXT CONSTRUCTION**

**SECURITY**

**PERFORMANCE COMPARISON**
初始化速度表现，存储表现， 查询速度表现， 交互带宽表现

**EVALUSTIONS**

**CONCLUSION**
还有脸方面工作可以继续探索：1、建立一个更安全的协议；1、将HXT应用到更多种类的查询中

## 扩展知识

### 可搜索加密技术 SE Searchable Encryption
可搜索加密问题源于文献[1]:假设用户Alice试图将个人文件存放在一个诚实但具有好奇心的外部服务器,以降低本地资源开销.为保护文件隐私,须采用某种加密方式将文件加密后存储.使用传统分组密码,只有密钥拥有者才具备解密能力,意味着Alice在执行基于关键词的查询操作时,需要下载所有已上传的文件,完全解密后再检索,会带来两个问题:① 如果Alice在服务器上已存有大量文件,一一下载会占用大量网络带宽,可能造成服务器堵塞;② 对已下载的所有文件完全解密会占用大量本地计算资源,效率极低.
解决此类问题的加密技术称为可搜索加密(searchable encryption,简称SE),该技术要求只有合法用户才具备基于关键词检索的能力.随着研究的推进,其应用并不仅限于此:2004年,Boneh提出使用非对称可搜索加密(asymmetric searchable encryption,简称ASE)解决“不可信赖服务器路由”问题[2];最近兴起的云计算[3]将是SE的最佳应用平台,由于服务提供商的不可控性,用户必须应对存储到云端的个人数据可能泄密的威胁,SE提供的加密和密文直接检索功能使服务器无法窃听用户个人数据,但可以根据查询
请求返回目标密文文件,这样既保证了用户数据的安全和隐私,又不会过分降低查询效率.

### 不经意交叉标签 OXT Oblivious Cross-Tag
TSet is cryptographic data structure that associates a list of fix length data tuples to each keyword in a database
TSet 是一个和数据库中关键词关联的固定长度的数据元组列表的加密数据结构

### Prime Order
素数阶
### r composite order bilinear pairings over elliptic curvegroups
椭圆曲线上的R阶复合双线性对，

## 读后感