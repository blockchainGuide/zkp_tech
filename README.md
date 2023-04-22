# zkp_tech
> 零知识证明

零知识证明技术在区块链领域可以提供隐私保护、效率提升、去中心化和数据完整性保护等优势。ZKP技术可以满足用户越来越严苛的安全需求，同时节约计算资源和时间，从而提高区块链技术的实用性和可靠性，尤其也是资方更青睐的技术点，本着学习以及应用的目的，开启了这个仓库，希望可以把这个过程中学习的知识做一个比较详细的整理，同时希望有兴趣的小伙伴可以共同贡献此仓库。

## 基本概念原理
### 密码学基础知识
#### 对称加密和非对称加密
#### 公钥密码学和私钥密码学
#### 哈希函数和数字签名
#### 完全同态加密（FHE）

### 零知识证明概念、历史和应用场景
#### 零知识证明的定义
#### 零知识证明的发展历程
#### 零知识证明的应用场景

### 零知识证明基本原理
#### 互模拟（simulators）
#### 可靠性（soundness）
#### 完整性（completeness）
#### 零知识性（zero-knowledgeness）

## 经典零知识证明协议

### Schnorr协议
#### Schnorr协议的原理和过程
#### Schnorr协议的安全性分析
#### Fiat-Shamir协议
#### Fiat-Shamir协议的原理和过程
#### Fiat-Shamir协议的安全性分析

### 非交互式零知识证明（NIZK）
#### 非交互式零知识证明的定义
#### Fiat-Shamir启发式方法
#### 非交互式零知识证明的应用

## 零知识证明构造
### 基于椭圆曲线密码学的零知识证明构造方法
#### 椭圆曲线密码学基础
#### 椭圆曲线上的零知识证明协议

### zk-SNARKs（Zero-Knowledge Succinct Non-Interactive Argument of Knowledge）
#### zk-SNARKs的概述
#### 多项式和椭圆曲线配对
#### Quadratic Arithmetic Programs (QAPs)
#### zk-SNARKs的构造过程

### zk-STARKs（Zero-Knowledge Scalable Transparent ARguments of Knowledge）
#### zk-STARKs的概述
#### 递归哈希和Merkle树
#### 低度扩展和多项式编码
#### zk-STARKs的构造过程

## 工程实践

- 实际项目使用零知识证明库：libsnark,bellman
- 阅读开源项目了解设计实现
- 了解零知识证明在隐私保护，安全计算的应用

## 流行的项目

- zkSync（Matter Labs） zkSync 是一个开源的、基于零知识证明的 Layer 2 扩展解决方案。它旨在提高以太坊网络的交易吞吐量和安全性
- Loopring Loopring 是一个去中心化交易协议，利用 zk-rollup 实现了高速、低成本的交易。它允许用户在链下进行交易，同时保持链上安全性。
- Aztec Network Aztec Network 是一个基于 zk-rollup 的隐私扩展解决方案，旨在提供高度可扩展的零知识证明技术以实现以太坊上的隐私交易
- StarkWare StarkWare 是一个基于零知识证明的扩展和隐私解决方案提供商。它的技术包括 StarkEx（用于扩展去中心化交易所）和 StarkNet（用于扩展整个以太坊网络）
- Hermez Network Hermez 是一个基于 zk-rollup 的 Layer 2 扩展网络，旨在提高以太坊的吞吐量和交易速度，降低手续费
- Scroll是以太坊上基于zkEVM的zkRollup，可实现现有以太坊应用程序和工具的本地兼容性
- Polygon zkEVM是第一个与以太坊虚拟机兼容的零知识扩展解决方案，用于集成智能合约和开发工具。
