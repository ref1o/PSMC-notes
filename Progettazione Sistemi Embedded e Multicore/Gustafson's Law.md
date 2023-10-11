A parallel platform does more than just speed up the execution of a sequential program. It can accommodate bigger problem instances.
Now suppose that $p$ processors take $T$ seconds ($T=T_{parallel}$) to run a job.
We have:$$T_{serial}=(1-\alpha)T+\alpha*p*T$$
$$S=\frac{T_{serial}}{T_{parallel}}$$
$$E=\frac{S}{p}=\alpha+\frac{1-\alpha}{p}$$
$S$ is also called *Scaled Speedup*.