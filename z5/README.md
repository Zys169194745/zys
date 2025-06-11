# 9.RNN

## 3.数据预处理验证
<img width="760" alt="91610388262da257e439494e595ed33" src="https://github.com/user-attachments/assets/da661cfa-4d0c-4557-88cd-2f0619725b2d" />





## 4.模型结构验证
<img width="740" alt="479ac7eba37b657e4fa80789c53494d" src="https://github.com/user-attachments/assets/f2915faf-defe-4c6e-a1ca-8c86af2b4e06" />




## 5.RNN序列处理验证
<img width="750" alt="414d34dc7862293ed9a4bb3b5c6d15b" src="https://github.com/user-attachments/assets/6892983d-b934-4511-a1af-a3ab476dbfe4" />


## 6.模型性能评估

## 7.推理能力验证
<img width="559" alt="208268297bc310d48a0791bc19467ad" src="https://github.com/user-attachments/assets/f675a007-0a24-4478-ab93-fe8581439d5e" />


# 10.RNN 



### 无条件姓氏生成

<img width="722" alt="67a945a777c10531532aa26582c32c3" src="https://github.com/user-attachments/assets/a4b56942-447b-4593-9a51-62ca5de94ca9" />

### 有条件姓氏生成

<img width="694" alt="8acac407f5906fc6d3d6f1871bf750b" src="https://github.com/user-attachments/assets/5a77650e-fff6-43e2-82c1-3a5673d9edaf" />

## 4、**回答问题**

① 两个模型的核心差异体现在什么机制上？  **B**

A. 字符编码方式不同

B. 是否考虑国家信息作为生成条件

C. RNN单元类型不同（GRU/LSTM）

D. 损失函数计算方式不同

② 在条件生成模型（Model2_Conditioned_Surname_Generation）中，国家信息通过什么方式影响生成过程？  **B**

A. 作为额外的输入特征拼接

B. 作为GRU的初始隐藏状态

C. 作为注意力机制的key

D. 作为输出层的偏置项

③ 文件2中新增的nation_emb层的主要作用是：  **B**

self.nation_emb = nn.Embedding(num_nationalities, rnn_hidden_size)

A. 将字符索引映射为稠密向量

B. 将国家标签转换为隐藏状态初始化向量

C. 生成姓氏的长度控制参数

D. 计算交叉熵损失的辅助参数

④ 对比两个文件的sample_from_model函数，文件2新增了哪个关键参数？  **B**

A. temperature

B. nationalities

C. device

D. max_length
