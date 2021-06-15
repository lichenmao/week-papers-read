## Revealing Every Story of Data in Blockchain Systems  

---

##### The problems

- 在现有的区块链中，查询数据的历史只能通过回放所有的交易记录进行。（**痛点问题**）
- 回放的方式对大规模，线下的分析可行。但不适合于在线的交易处理。

##### Main contributions

- LineageChain： 一个面向区块链的细粒度，安全和有效的回溯系统。
- 提供简单的接口，能够使得在运行时依赖于出处信息的区块链程序能够更加快速。
- 在合约执行时获取出处，并将信息存储在Merkle树中。
- 提供了一个新的 skip list index 来支持有效的出处查询系统。
- provenance。

##### Smart Contract APIs

目前的智能合约仅能够利用最新的状态，而LineageChain通过三个额外的智能合约APIs提供对获取的来源信息的访问。

- Hist
- Backward
- Forward





