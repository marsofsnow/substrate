
# v3.0.0
learn

# primitives
Runtime Primitives是一组基础类型，是构成Substrate runtime基础元素，分为核心类型（Core Primitives）和框架类型（FRAME Primitives）。
# frame
Substrate提供一些预置模块，这些pallet具有足够的通用性，可供许多区块链重复使用。

Substrate v2.0.0的所有预置模块列在下表中（点击模块名可以查看文档）：

模块名	源码	功能
assets	源码	处理同质化资产（fungible assets）
atomic_swap	源码	原子性的资金交换协议
aura	源码	通过管理离线报告扩展Aura共识
authority_discovery	源码	检索当前的权限集，了解其拥有的权限ID，签署和验证与其他权限之间的消息
authorship	源码	跟踪区块的当前生产者和最近叔块
babe	源码	通过从VRF（可验证随机函数）的输出中收集链上的随机性，并管理epoch转变，来扩展BABE共识
balances	源码	处理账户和余额
benchmark	源码	以隔离的方式包含常见的runtime模式，此模块不用于生产环境，仅用于基准测试
collective	源码	允许一组帐户ID通过专门来源的分发调用来使它们集体公开
contracts	源码	部署和执行WebAssembly智能合约
democracy	源码	提供一种民主制度，处理一般利益相关者的投票管理
elections	源码	基于抵押权重的选举模块
elections_phragmen	源码	基于Sequential Phragmén的选举模块
evm	源码	以太坊虚拟机（EVM）执行模块
example	源码	示例模块，展示了大多数pallet共有的概念、API和结构
example_offchain_worker	源码	示例模块，展示了大多数链下工作机共有的概念、API和结构
grandpa	源码	通过管理为native代码准备的GRANDPA权限来扩展GRANDPA共识
identity	源码	一个联合name系统，允许从指定来源添加多个注册商，注册服务商可以收取一定费用以提供身份验证服务
im_online	源码	允许验证人在每个新会话中发送心跳，以表明该节点处于连接状态
indices	源码	为新创建的帐户分配索引，索引是地址的缩写形式
membership	源码	允许控制一组AccountId的成员资格，用于管理集合体的成员资格
multisig	源码	进行多重签名分发
nicks	源码	用于在链上跟踪账户名，无需创建name层次结构、替换DNS或提供反向查找
node_authorization	源码	管理许可网络的一组可配置节点
offences	源码	跟踪报告的作恶行为
proxy	源码	代理，允许账户授予其他账户许可，以从其签名来源分发调用类型
randomness_collective_flip	源码	提供可以在测试中使用的随机函数，根据前81个区块的哈希值生成影响较小的随机值，此模块不用于生产环境
recovery	源码	一种M-of-N社交恢复工具，在私钥或其他身份验证机制丢失时用户也可以访问其账户
scheduler	源码	以指定区块高度或指定周期发生的计划表
scored_pool	源码	维护一个积分池，得分最高的实体成为会员
session	源码	允许验证人管理其会话密钥，提供更改会话长度、处理会话轮换的功能
society	源码	一个鼓励用户参与和维护会员制社会的经济学游戏
staking	源码	管理网络维护者抵押的资金
sudo	源码	允许单个账户执行需要root权限的可调度功能
timestamp	源码	获取和设置链上时间
transaction_payment	源码	提供计算分发前交易费用的基本逻辑
treasury	源码	提供可以由系统中的利益相关者管理的资金池，以及从该资金池提出支出建议的结构
utility	源码	一个带有助手的无状态模块，用于调度管理
vesting	源码	提供一种在账户的锁定余额上放置线性曲线的方法，该模块确保有一个锁定位置，防止余额因交易费用支付以外的任何原因而降至未投资额以下

##  生成文档

cargo doc --open 
