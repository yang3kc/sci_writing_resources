Here I list some tricks I use when writing

# LaTeX

## Fix table overflow
If your table is too big, the `resizebox` command can be very handy:
```tex
\begin{table*}
    \centering
    \caption{Detailed information about different groups of accounts in \dataset{TwitterGAN}.}
    \resizebox{\textwidth}{!}{
        \begin{tabular}{ll}
        \hline
        Name 1 & Name 2 \\
        \hline
        Value 1 & Value 2 \\
        \hline
        \end{tabular}
    }
    \label{tab:my_table}
\end{table*}
```
