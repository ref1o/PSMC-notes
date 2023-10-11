Unless virtually all of a serial program is parallelized, the possible speedup is going to be very limited, regardless of the number of cores available

Now suppose that 1 processor take $T$ seconds ($T=T_{serial}$) to run a job. The application consists of a $0\leq\alpha\leq1$ part that can be parallelized. The remaining $1-\alpha$ has to be done sequentially.
$$T_{parallel}=(1-\alpha)T+\frac{\alpha T}{p}$$
$$S=\frac{T_{serial}}{T_{parallel}}=\frac{T}{(1-\alpha)T +\frac{\alpha T}{p}}=\frac{1}{(1-\alpha)+\frac{\alpha}{p}}$$
$$\lim_{p\to\infty}S=\frac{1}{1-\alpha}$$
###### Ex. 
We can parallelize 90% of a serial program. Parallelization is "perfect" regardless of the number of cores $p$ we use. $T_{serial}$ = 20 seconds.
The runtime of the parallelizable part is:$$\frac{0.9*T_{serial}}{p}=\frac{18}{p}$$
The runtime of the unparallelizable part is:$$0.1*T_{serial}=2$$
The overall parallel runtime is:$$T_{parallel}=\frac{0.9*T_{serial}}{p}+0.1*T_{serial}=\frac{18}{p}+2$$
The speedup:$$S=\frac{T_{serial}}{\frac{0.9*T_{serial}}{p}+0.1*T_{serial}}=\frac{20}{\frac{18}{p}+2}$$
