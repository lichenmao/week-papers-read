#### CAPER: A Cross-Application Permissioned Blockchain

> Amiri, Mohammad Javad, Divyakant Agrawal, and Amr El Abbadi. "Caper: a cross-application permissioned blockchain." *Proceedings of the VLDB Endowment* 12, no. 11 (2019): 1385-1398.

----

#### Abstract

尽管最近进行了深入的研究，现有的区块链系统还不能够充分的解决所有的分布式应用的特性。尤其是，分布式应用根据服务级别协议（SLAs）相互间协作来提供不同的服务。当应用间进行协作时，例如.,跨应用交易，应当被所有应用可见，但是每个应用程序间的数据（例如，内部事务）可能是机密。在本文中，我们介绍了CAPER——一种许可链系统，**能够支持协同分布式应用的内部和跨应用的事务**。在CAPER中，区块链账本形成了一个有向无环图，其中每个应用仅访问和维护自己的账本视图，包括了其内部和所有与其他应用的事务。CAPER还引入了三种共识协议，全局的对具有不同内部共识协议的应用间的交易进行排序。实验的结果展示了CAPER在性能和可扩展性方面的效果。

#### Main contribution

- 引入了区块链了视图。每个应用仅可以维护自己的账本视图，包括了内部和所有跨应用的交易。
- CAPER，一个支持协同分布应用的许可链。CAPER同时支持内部和跨应用交易。
- 三种不同的共识协议，用于在具有不同局部共识协议的应用程序之间的交易进行全局排序。

#### Question

- 每个应用都只可以看到自己的账本视图，是否违背了区块链的透明性原则。如何确保数据的一致性。
- **我的一个设想。是会再出来一个账本，记录各应用数据的Hash码（方便联盟中的成员验证数据是否篡改），类似于私有云， 实现在物理上或者逻辑上的隔离，让其他的用户不能看到自己的交易，只可以验证**

#### Significant limitations of permissioned blockchain

- poor performance
- lack of confidentiality
- Inefficient cross-application transcation support







