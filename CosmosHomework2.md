# Cosmos-2
一、选择题（单选/多选）
1、以下哪个组件会将合法的 Tx 通过 P2P 网络广播给其它节点？  B  
A. AnteHandler  
B. Mempool  
C. Mempool Cache  
D. ABCI  
2、如果一个区块高度没有达成共识，Cosmos 区块链会如何处理？  C  
A. 跳过没有达成共识的区块，在下一个区块高度重新共识  
B. 在当前区块高度、当前 Round 中继续等待  
C. 在当前区块高度的下一个 Round 中重新共识  
D. 共识失败，区块链节点停止运行  
3、关于 Staking 模块，以下哪种说法是正确的？  
A. 验证人作恶，其委托人也会受到惩罚  AC
B. 验证人收到的委托越多，共识投票的权重就越高  
C. 验证人向委托人收取的佣金比例是 Cosmos 区块链系统参数决定的  
D. 委托人需要运行区块链节点才能“挖矿”  
4、哪种场景会触发一个验证人的所有委托人的收益取回？  D  
A. 委托人提取收益时  
B. 验证人提取收益时  
C. 委托人执行委托、解委托或转委托时  
D. 验证人修改佣金比例时  
5、对于验证人双签的惩罚可能有哪些？  ACD  
A. 根据链上参数，罚没验证人和其委托人的委托通证总量的对应比例  
B. 根据链上参数，仅罚没验证人自委托通证的对应比例  
C. 在一段时间内，禁止该验证人继续参与共识  
D. 永久禁止该验证人继续参与共识  
6、哪些人可以参与 Cosmos 区块链的链上提案治理投票？  AB  
A. 验证人  
B. 委托人  
C. Native 通证持有人  
D. 任何人  
7、以下哪些更新操作是“共识”非兼容的？  AB
A. 加载新的功能模块  
B. 数据的存储结构变更  
C. AnteHandler 逻辑更新  
D. REST API 结构非兼容更新  

二、问答题
1、为什么 Distribution 模块设计为“被动”的方式分发收益？  
答：因为 Token 的增发是在每一个区块里进行的，每个区块都会产生收益，这些收益最终被打包到一个区块中结算，如果主动地在每个区块里进行收益结算，会给整个网络带来很大的性能压力。  
2、为什么非兼容的软件版本升级时，要确保所有的节点在相同的区块高度执行升级？  
答：让所有的节点在相同的状态基础上升级软件版本，达成新的共识。  
3、OPEN Sea 的 Metadata 规范？  
答：{
  "description": "Friendly OpenSea Creature that enjoys long swims in the ocean.", 
  "external_url": "https://openseacreatures.io/3", 
  "image": "https://storage.googleapis.com/opensea-prod.appspot.com/puffs/3.png", 
  "name": "Dave Starbelly",
  "attributes": [ ... ]
}
