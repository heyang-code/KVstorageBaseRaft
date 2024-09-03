# KVstorageBaseRaft
# cpp实现的基于Raft算法的k-v存储数据库
# 分支说明
main：实现一个简单的clerk  
rpc：muduo和rpc框架相关内容  
raft_DB：基于Raft的k-v存储数据库，主要用于观察选举过程  
本项目主要是学习Raft的原理，并实现一个简单的k-v存储数据库
# 项目文档目录说明
1	2	3	4

# 项目编译运行
Cmake一键编译启动
mkdir cmake-build-debug
cd cmake-build-debug
cmake ..
make

