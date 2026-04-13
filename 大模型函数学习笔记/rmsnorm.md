# 计算$\sigma$


# 计算$\hat{x_i}$
已知$\sigma,w$，计算$\hat{x_i}$。
取4x8行32列的向量(bf16) ,8维fp32的$\sigma$, 2x64维bf16的w;
首先将$\sigma$拆分成两组，在一个向量寄存器中可以存储128个
