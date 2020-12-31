# LaTeX Guidelines for the Final Report
Version on Dec 31, 2020.

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

To refer to a equation, in the text simply do:
```tex
Equation~\eqref{eq:XX}
```

To refer to a section, in the text simply do:
```tex
Section~\ref{sec:XX}
```

In the text, start referring to the figure, section, equation *with a **capital** letter*, please.

Example: 

```tex
In Section~\ref{sec:XX} from Figure~\ref{fig:XX}, we can observe that ...
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

6. Finish the itemizations/enumerations with a punctuation (meaning "Do not forget the full stop (.)!" in most of the cases).

Example:
```tex
\begin{itemize}
\item The Speaker has the power to:
    \begin{enumerate}
    \item announce the result of an election.
    \end{enumerate}
\end{itemize}
```

7. When you **define** a terminology related to your section, you are advised to use `\begin{definition} ... \end{definition}`. A `definition` theorem-like environment will be defined in the report

Example:
```tex
\begin{definition} \label{def:ballot}
    A \textbf{ballot} is related to each island's \textbf{power} to support or disagree with the rule specified in the vote called by the President. 
\end{definition}
```

8. Write "i.e. ..... e.g. ..", NOT "i.e., ..... e.g., ..". I personally think comma is very unnecessary for these abbreviations.

9. Use comma appropriately! A common mistake is to *forget* using comma before "FANBOYS" which are:
- for
- and
- nor
- but
- or
- yet
- so

Note that "FANBOYS" are used to connect *clauses*. 

10. Do NOT use comma before "and" for the case of connecting words.

Example:
```tex
$X$, $Y$ and $Z$ are variables that define....
```
Note that there is no comma before "and" in this case -- as this "and" is connecting the *nouns* and therefore, not the same "and" in FANBOYS which are indicated in point 9. 

11. Use full stops appropriately with commas. If the quote can be conceptually replaced by emphasis/bold text, then the full stop should be outside the quotation marks (see Example 2 below). If the sentence ends within the quote the full stop should be inside the quote (see Example 1 below).
Example 1:
According to Byron, "Our burgers are fantastic."
Example 2:
 The LaTeX guidelines are "fun".


## Todo:
Write more guidelines as we progress...