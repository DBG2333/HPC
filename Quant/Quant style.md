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
量化前的数列A的abs(最大值,最小值)和数列B的abs(最大值,最小值)对应
$$max(abs(a_{min}),abs(a_{max}))->max(abs(b_{min}),abs(b_{max}))$$

scale放缩系数记为：
$$s=\frac{max(abs(a_{min}),abs(a_{max}))}{max(abs(b_{min}),abs(b_{max}))}$$
**非对称量化**指的是量化后的数列使用到了数据类型的上下限

量化后的数列B的最大值和最小值和int8的范围对应
$$a_{min}->b_{min}=min(int 8)\quad a_{max}->b_{max}=max(int 8)$$

scale放缩系数记为：
$$s=\frac{a_{max}-a_{min}}{max(int 8)-min(int 8)}$$
# Quant in LLM
对于Weight做量化，Activation不量化
假设存在 
$$
\begin{align*}
z=a_1w_1+a_2w_2\\
\hat z=a_1\hat w_1+a_2\hat w_2\\
\Delta z=a_1\Delta w_1+a_2\Delta w_2
\end{align*}$$



# GPTQ


# AWQ

