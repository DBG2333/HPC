# Basic quant
原数列A
$a_{min}=min(A)\quad a_{max}=max(A)$
规定量化后的数列 B数据类型，以int8举例，其数值范围为：
$$max(int 8)=2^7-1 \quad min(int 8)=-(2^7-1) $$
**零点**指的是量化前的0，对应量化后的数值

**对称量化**指的是量化后的零点取在值域中点
对称量化下：
量化的数据类型如果是有符号数，零点一般是0（如int8 int4）
量化的数据类型如果是无符号数，零点一般取中点（UINT8->0~255 ）
量化后的数列B的最大值和最小值和int8的范围对应
$$a_{min}->b_{min}=min(int 8)\quad a_{max}->b_{max}=max(int 8)$$

scale放缩系数记为：

**非对称量化**指的是量化后的数列使用到了数据类型的上下限

量化后的数列B的最大值和最小值和int8的范围对应
$$a_{min}->b_{min}=min(int 8)\quad a_{max}->b_{max}=max(int 8)$$

scale放缩系数记为：
$$s=\frac{a_{max}-a_{min}}{max(int 8)-min(int 8)}$$




# GPTQ


# AWQ

