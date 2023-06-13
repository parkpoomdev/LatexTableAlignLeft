# LatexTableAlignLeft
In this repository record the table format for latext in IEEE paper. The table align is center and the align of the text in table is left.

```latex
\documentclass{article}
\usepackage{array} 

\begin{document}

% Define the padding for the table cells
\setlength{\tabcolsep}{5pt} % horizontal padding
\renewcommand{\arraystretch}{1.5} % vertical padding

\begin{table}[!ht]
\caption{Comparative Study}
\begin{center}
\begin{tabular}{|>{\raggedright\arraybackslash}p{1.7cm}|>{\raggedright\arraybackslash}p{1.6cm}|>{\raggedright\arraybackslash}p{1.6cm}|>{\raggedright\arraybackslash}p{1.6cm}|}
\hline
\textbf{Factor} & \textbf{No-code} & \textbf{Low-code} & \textbf{High-code} \\ \hline
Technical Expertise & Little to none & Some coding expertise & Significant coding expertise \\ \hline
Customization & Limited & More options & Maximum \\ \hline
Flexibility & Most flexible & Flexible & Least flexible \\ \hline
Scalability & Limited & Good for mid-level applications & Best for complex and scalable applications \\ \hline
Cost & Least expensive & Less expensive than high-code & Most expensive \\ \hline
Maintenance & Requires less maintenance & Requires some maintenance & Requires more maintenance \\ \hline
\end{tabular}
\end{center}
\label{compare_table}
\end{table}

% Reset the padding for the table cells (optional)
\setlength{\tabcolsep}{6pt} % default
\renewcommand{\arraystretch}{1.0} % default

\end{document}
```
