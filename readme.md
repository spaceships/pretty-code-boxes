pretty-code-boxes
=================

![picture!](https://raw.githubusercontent.com/spaceships/pretty-code-boxes/master/pic.png)

My take on code listings in latex.

Usage:
------

```
\begin{codebox}{$\mathsf{Gb}'(C, \{s_i\}_{i \in [q^{2d}]}, x_1, \delta_1, \cdots, x_n, \delta_n)$}
    \comment{Combine the \delta{}s using addition mod $q^{2d}$}\\
    $\Delta = \{ \sum_{j \in [\lambda]}  \delta_{i,j} \mod q^{2d}\}_{i \in [n]}$\\
    \\
    \comment{Combine the seeds using \Delta}\\
    $r = \bigoplus_{i \in [\lambda]} s_{\Delta_i}$\\
    \\
    \comment{Call \textsf{Gb} and \textsf{En} using $r$}\\
    return $\Gb(C; r),\, \En(x_1 || \dots || x_n; r)$
\end{codebox}
```
