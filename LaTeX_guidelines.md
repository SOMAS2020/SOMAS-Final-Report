# LaTeX Guidelines for the Final Report
Version on Dec 24, 2020.

Author: Ezgi.

Assuming that anyone has some sort of familiarity with LaTeX, these are meant to be just *friendly reminders* about how to write the final report.

1. In the report, we need to label *everything* that we refer to: figures, equations, sections, subsections, subsubsections etc. 

For figures, do:
```tex
\label{fig:XX}
```
For equations, do:
```tex
\label{eq:XX}
```
For sections, do:
```tex
\label{sec:XX}
```
For subsections, do:
```tex
\label{subsec:XX}
```
I hope you get the idea :)

To refer to these labels, let's say a figure, in the text simply do:
```tex
Figure~\ref{fig:XX}
```

2. Write *proper* captions for your images! (Sometimes, people don't do this for some reason that I don't understand...)  Finish your caption with a punctuation, please.

Example:
```tex
\begin{figure}[H]
...
\caption{Transfer-of-power cycle.}
\end{figure}
```

3. Footnotes appear *before* the punctuation.

Example:
```tex
... at each turn\footnote{It is assumed that...}.
```

4. `\texttt{}` style is only for referring to something related to code.

Example:
```tex
... \texttt{update_island()} updates resources of each island.
```

5. When referring to anything mathematical (e.g. variables, simple equations), write them in the math mode using `$ $`.

Example:
```tex
... the island $X$ has taken $Y$ amount of resources such that ...
```


## Todo:
Write more guidelines as we progress...