# 数据预处理验证
<img src="images/data_solve.png" width="800" alt="数据预处理验证">
<img width="502" alt="65b73a0333c2af0baf372eef8242d59" src="https://github.com/user-attachments/assets/2bf7b3b9-5221-4e7a-b6e4-6b11d3086e7d" />

# 模型结构验证
<img src="images/model.png" width="800" alt="模型结构验证">
<img width="503" alt="0976e2bb72dacb410ca1192b9226757" src="https://github.com/user-attachments/assets/f0910703-a6a3-4dd4-95de-6f1c5b7320b5" />

# RNN序列处理验证
<img src="images/RNN_seq.png" width="800" alt="RNN序列处理验证">
<img width="482" alt="e32ba8d5c743b12b4a5ca3451103c97" src="https://github.com/user-attachments/assets/1ec90a00-dd72-4d9e-a35a-b2e40c495a59" />

# 50轮损失值
<img src="images/evalution.png" width="800" alt="50轮损失值">
<img width="505" alt="52490bef09043f4a13a04079fc3e609" src="https://github.com/user-attachments/assets/2a530077-0326-4be0-9fd3-7bd069bc9c29" />

# 推理结果

<img width="487" alt="74cbc9d6bb73eff43e190b8117a98ae" src="https://github.com/user-attachments/assets/302f3f05-6ecb-4cab-ae47-61ab52a21734" />

# 无条件生成姓氏
<img width="485" alt="dac65c35b922f5b717e3797851e299e" src="https://github.com/user-attachments/assets/20eb6cf0-7ff9-468d-a1e2-bc0e13d05664" />


# 有条件生成姓氏
<img src="images/Conditioned.png" width="800" alt="有条件生成姓氏">
<img width="494" alt="a6e5320162ae04b7f18ade148edf42a" src="https://github.com/user-attachments/assets/8b7ceb36-a956-43b2-95c7-8ba746c04097" />

# 问题答案
1、两个模型的核心差异体现在什么机制上？（ B ）\
A. 字符编码方式不同\
B. 是否考虑国家信息作为生成条件\
C. RNN单元类型不同（GRU/LSTM）\
D. 损失函数计算方式不同

2、在条件生成模型（Model2_Conditioned_Surname_Generation）中，国家信息通过什么方式影响生成过程？（ B ）\
A. 作为额外的输入特征拼接\
B. 作为GRU的初始隐藏状态\
C. 作为注意力机制的key\
D. 作为输出层的偏置项

3、文件2中新增的nation_emb层的主要作用是：（ B ）\
self.nation_emb = nn.Embedding(num_nationalities, rnn_hidden_size)\
A. 将字符索引映射为稠密向量\
B. 将国家标签转换为隐藏状态初始化向量\
C. 生成姓氏的长度控制参数\
D. 计算交叉熵损失的辅助参数

4、对比两个文件的sample_from_model函数，文件2新增了哪个关键参数？（ B ）\
A. temperature\
B. nationalities\
C. device\
D. max_length
