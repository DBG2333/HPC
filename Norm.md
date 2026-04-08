# Layer-norm
对于向量$X=[x_1,\cdots,x_n]^T$做归一化
$$
\begin{align*}
&\mu=\frac{\Sigma x_i}n\\
&\sigma=\sqrt\frac{\Sigma(x_i-\mu)^2}{n}\\
&\hat{x_i}=\gamma \frac{x_i-\mu}{\sigma+\epsilon}+\beta
\end{align*}
$$
# RMS-norm
不做均值，直接计算
$$
\begin{align*}
&\sigma=\sqrt\frac{\Sigma x_i^2}{n}\\
&\hat{x_i}=\gamma\frac{x_i}{\sigma}
\end{align*}
$$