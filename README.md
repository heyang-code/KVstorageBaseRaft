# KVstorageBaseRaft
# cpp实现的基于Raft算法的k-v存储数据库
# 分支说明
main：实现一个简单的clerk  
rpc：muduo和rpc框架相关内容  
raft_DB：基于Raft的k-v存储数据库，主要用于观察选举过程  
本项目主要是学习Raft的原理，并实现一个简单的k-v存储数据库
# 项目文档目录说明
├── bin 生成的可执行文件存放地
├── cmake-build-debug 项目编译目录，默认是没有的，需要自己创建
├── docs    项目文档存放地
├── example  范例代码存放地
│   ├── fiberExample  协程相关代码
│   ├── raftCoreExample raft核心代码
│   └── rpcExample rpc相关代码
├── lib  项目编译后的库文件存放地
├── src 【重点】项目源代码存放地，按照子模块组织
│   ├── common  子模块共用的，一般是一些util，日志，配置文件
│   ├── fiber  协程相关代码
│   ├── raftClerk raft客户端代码
│   ├── raftCore raft核心代码
│   ├── raftRpcPro raft中rpc涉及的protoc文件
│   ├── rpc  rpc库相关代码
│   └── skipList 跳表（上层状态机）相关代码
└── test  测试代码存放地，作用不大，一般是对一些不确定的特性进行测试
# 项目编译运行
Cmake一键编译启动
mkdir cmake-build-debug
cd cmake-build-debug
cmake ..
make

