# Awesome DAG Blockchain

[![](https://camo.githubusercontent.com/13c4e50d88df7178ae1882a203ed57b641674f94/68747470733a2f2f63646e2e7261776769742e636f6d2f73696e647265736f726875732f617765736f6d652f643733303566333864323966656437386661383536353265336136336531353464643865383832392f6d656469612f62616467652e737667)](https://github.com/sindresorhus/awesome)
[![](https://camo.githubusercontent.com/cb8cb80af654f3dae14a4aa62e44bf62f16953d6/68747470733a2f2f6a617977636a6c6f76652e6769746875622e696f2f73622f6c616e672f6368696e6573652e737667)](README.md)
[![](https://camo.githubusercontent.com/15a53d5ec5d896319068168a27da0203156bbdb9/68747470733a2f2f6a617977636a6c6f76652e6769746875622e696f2f73622f6c616e672f656e676c6973682e737667)](README-en.md)

这个仓库主要是用来搜集与基于DAG技术的区块链相关的资源，请随意Star或者Fork。如果有任何建议和评论，[请提交到这里](https://github.com/guantau/Awesome-DAG-Blockchain/issues)。欢迎提交各种PR :)，格式参考 [awesome](https://github.com/sindresorhus/awesome) 的清单。

[中文](README.md) | [English](README-en.md)

## 目录

+ [主要论文](#主要论文)
+ [典型实现](#典型实现)
+ [技术对比](#技术对比)
+ [相关人物](#相关人物)




## 主要论文

+ [NXT论坛DAG帖](https://nxtforum.org/proof-of-stake-algorithm/dag-a-generalized-blockchain/) - 2014年帖子，需登录查看
+ [DAGCoin](https://bitslog.files.wordpress.com/2015/09/dagcoin-v41.pdf) - 2015年由Sergio Demian Lerner提出，但并没有代码实现
+ [Accelerating Bitcoin’s Transaction Processing. Fast Money Grows on Trees, Not Chains.](https://eprint.iacr.org/2013/881.pdf) - 2013年由提出修改Bitcoin协议，从而加快确认速度
+ [Inclusive Block Chain Protocols](http://www.cs.huji.ac.il/~avivz/pubs/15/inclusive_btc.pdf) - 2015年提出DAG模型
+ [SPECTRE:Serialization of Proof-of-work Events: Confirming Transactions via Recursive Elections.](https://eprint.iacr.org/2016/1159.pdf) - 基于DAG的分布式账本
+ [PHANTOM: A Scalable BlockDAG protocol](https://eprint.iacr.org/2018/104.pdf)  - 解决了blockDAG全序的问题
    + [部分译文 by DAGfans](https://github.com/DAGfans/TranStudy/blob/master/Papers/PHANTOM%20-%20A%20Scalable%20BlockDAG%20protocol.md)


## 典型实现

### IOTA

+ 简介：面向物联网应用
+ [官网](https://iota.org/)
+ [白皮书](https://iota.org/IOTA_Whitepaper.pdf)
+ [代码库](https://github.com/iotaledger)

### Byteball

+ 简介：面向日常支付使用，具有简单的智能合约
+ [官网](http://byteball.org/)
+ [白皮书](https://byteball.org/Byteball.pdf)
+ [代码库](https://github.com/byteball)
+ 相关资源：
  + [byteball介绍1](https://medium.com/@Suirelav/introduction-to-byteball-part-1-why-ab3ff6a7a8f2) - byteball的产生原因
  + [byteball介绍2](https://medium.com/@Suirelav/introduction-to-byteball-part-2-the-dag-ce84ca4c4e01) - DAG技术
  + [byteball介绍3](https://medium.com/@Suirelav/introduction-to-byteball-part-3-smart-contracts-81efa010a0b3) - 智能合约
  + [byteball介绍4](https://medium.com/@Suirelav/introduction-to-byteball-part-4-adoption-ff37d87615c9) - byteball的各种应用
  + [byteball原理解析1](http://blog.guantau.com/2017/12/14/byteball1/) - DAG数学基础及byteball区块链结构
  + [byteball原理解析2](http://blog.guantau.com/2017/12/19/byteball2/) - byteball的共识算法
  + [byteball原理解析3](http://blog.guantau.com/2018/01/19/byteball3/) - byteball的地址、脚本及合约
  + [byteball原理解析4](http://blog.guantau.com/2018/01/26/byteball4/) - byteball的网络结构
  + [byteball原理解析5](http://blog.guantau.com/2018/01/30/byteball5/) - byteball的应用
  + [byteball主网压力测试](https://blog.goodaudience.com/byteball-main-net-under-stress-test-c131ba85b72b) - 测试给出了三点结论：（1）交易处理速度仅能达到15TPS左右，不同于传统区块链交易处理速度受限于区块大小，DAG网络的交易处理速度与代码执行速度、网络传输时延、硬件处理能力等都可能有关系；（2）网络容易遭受DOS攻击，大量突发式的恶意交易会阻塞网络，降低网络的交易处理速度；（3）随着交易数量增加，交易确认时间可以保持平稳。

### NANO

+ 简介：早期称为RaiBlocks，最早在2014年发布beta测试
+ [官网](https://nano.org/)
+ [白皮书](https://nano.org/zh/whitepaper)
+ [代码库](https://github.com/nanocurrency)
+ 相关资源：
  + [RaiBlocks网络压力测试1](https://hackernoon.com/stress-testing-the-raiblocks-network-568be62fdf6d)
  + [RaiBlocks网络压力测试2](https://medium.com/@bnp117/stress-testing-the-raiblocks-network-part-ii-def83653b21f)

### DAGCoin

+ 简介：基于Byteball代码进行修改
+ [官网](https://dagcoin.org/)
+ [白皮书](https://dagcoin.org/whitepaper.pdf)
+ [代码库](https://github.com/dagcoin/)

### TrustNote

- 简介：基于Byteball代码进行修改
- [官网](https://trustnote.org/)
- [白皮书](https://trustnote.org/TrustNote-WhitePaper.pdf)
- [代码库](https://github.com/trustnote)

### Nerthus

- 简介：基于DAG通用的智能合约编程平台与区块链操作系统
- [官网](http://nerthus.io/)
- [白皮书](http://nerthus.io/static/downfile/NerthusWhitePageV0.0.2.pdf)

### AskCoin（已死）

- 简介：基于DAG的知识付费
- [尸体](https://blog.askcoin.org/askcoin-in-one-page-f284bb3d9b42)

### IOT Chain

- 简介：使用PBFT+DAG
- [官网](https://iotchain.io/)
- [白皮书](https://iotchain.io/whitepaper/ITCWHITEPAPER.pdf)
- [代码库](https://github.com/IoTChainCode)

### XDAG

- 简介：可以挖矿
- [创世贴](https://bitcointalk.org/index.php?topic=2552368.0)
- [官网](http://xdag.io/)
- [白皮书](https://docs.google.com/document/d/1ruNpTVghy0Xsb8gOa-8sYG58GHU_ibeGnwJi2h0TTnA/edit)

### HashGraph

+ 简介：一种新型的DAG技术
+ [官网](https://hashgraph.com/)
+ [白皮书](https://www.swirlds.com/downloads/SWIRLDS-TR-2016-01.pdf)
+ 代码库：
  + [Python实现](https://github.com/Lapin0t/py-swirld)
  + [NodeJS实现](https://github.com/TheCallSign/hashgraph)
  + [Go实现](https://github.com/babbleio/babble)

### 其它

+ [daglabs](https://www.daglabs.com/) - 主要实现SPECTRE和PHANTOM两种DAG上的共识算法




## 技术对比

+ [IOTA vs RaiBlocks](https://hackernoon.com/iota-vs-raiblocks-413679bb4c3e)
+ [DAG coin comparison (Byteball, IOTA, RaiBlocks, etc)](https://web.archive.org/web/20171211100146/https://www.reddit.com/r/CryptoCurrency/comments/7iv20r/dag_coin_comparison_byteball_iota_raiblocks_etc/)




## 相关人物

+ Sergio Demian Lerner
+ Yonatan Sompolinsky
+ Yoad Lewenberg
+ Aviv Zohar
+ Serguei Popov
+ Sergey Ivancheglo
+ Anton Churyumov
+ Leemon Baird
