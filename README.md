# DDPG-UAV

首先感谢您百忙之中抽空帮忙，您在测试的过程中需要创建五个文件夹，他们分别是loss_ddpg,net_file,network_data,reward_data,test_data。
代码大致逻辑为在训练过程中，每一循环都保证路径不会重复，且100次循环找出一个最好的路径放入buffer中以供训练
测试时直接调用训练好的网络
但是现在的情况就是在训练时可以看到效果很好，一到测试他网络的输出基本不变
