\documentclass{beamer}
\usepackage{amsmath}
\usepackage{multirow}
\usepackage{graphicx}
\usetheme{Pittsburgh}  
\setbeamercolor{background canvas}{bg=blue!2}
\setbeamercolor{titlelike}{bg=teal,fg=white}
\setbeamercolor{block title}{bg=blue!20,fg=black}
\setbeamercolor{frametitle}{bg=teal,fg=white}
\setbeamertemplate{blocks}[rounded][shadow=true]
\title{\textbf{\underline{\fontsize{10pt}{20pt}\selectfont {\fontfamily{cmtt} \selectfont{SEC1: Document Preparation and  Presentation Software}}}}}
\author{\textbf{Sonia}\\
\fontfamily{cmtt} \selectfont{\fontsize{10pt}{20pt}\selectfont {Roll no. - 2022346 \\
BSc. Hons Computer Science }}}
\institute{\textit{\textcolor{teal}{\fontfamily{qag} \selectfont{Shaheed Rajguru College of Applied Sciences for women \\ (University of Delhi)}}}}
\date{\today}
\begin{document}
\begin{frame}
\begin{figure}
    \centering
    \includegraphics[width=8cm,height=3cm]{latex.jpg}
\end{figure}
    \titlepage
\end{frame}
\begin{frame}{\fontfamily{cmtt} \selectfont{\fontsize{10pt}{20pt} \selectfont {TABLE OF CONTENTS}}}
 \begin{block}{}
     \tableofcontents
 \end{block}  
\end{frame}
\begin{frame}{\fontfamily{cmtt} \selectfont{\fontsize{10pt}{20pt} \selectfont {LIMITS OF FUNCTIONS}}}
\begin{block}{}
\fontsize{10pt}{10pt} \selectfont{
      \section{Limits of functions}
In this section, we will introduce the important notion of the limit of a function. The intuitive idea of the function \textit{f} having a limit \textbf{L} at the point c is that the values $ \textit{f}(x) $ are close to \textbf{L} when x is close to (but different from) c. But it is necessary to have a technical way of working with the idea of "Close to" and this is accomplished in the $\varepsilon-\delta$ definition given below. \\
In order for the idea of the limit of a function \textit{f} at a point c to be meaningful,it is necessary that \textit{f} be defined at points near c. It need not be defined at the point c,but it should be defined at enough points close to c to make the study interesting . This  is the reason for the following definition. }
\end{block}
\begin{block}{}
    \begin{figure}[h]
    \centering
    \includegraphics[width=8cm]{limit-notation-explanation.png}
    \caption{Basic Terms in Limits}
    \label{}
\end{figure}
\end{block}
\end{frame}
\begin{frame}
    \begin{columns}
    \begin{column}{.48\textwidth}
     \begin{block}{}
    \fontsize{8pt}{10pt} \selectfont{
   \subsection{Definition}
Let $A \subset \mathbf{R}$. A point $ \textit{c} \in \mathbf{R}$ is a \textbf{Cluster point} of A if for every $\delta > 0$ there exists at least one point $x \in A, x\neq c$ such that $\mod{x-c} < \delta $.
This definition is rephrased in the language of neighborhoods as follows : A point c is a cluster point of the set A if every $\delta$-neighborhood $V_\delta(c)=(c-\delta,c+\delta)$ of c contains at least one point of A distinct from c.\\
\textbf{Note}\: The point c may or may not be a member of A, but even if it is in A,it is ignored when deciding whether it is a cluster point of A or not, since we explicitly require that there be points in $V_\delta(c)\cap A$ distinct from c in order for c to be a cluster point of A.\\
For example, if $A:= {1,2}$,then the point 1 is a cluster point of A, since choosing 
$\delta :=\frac{1}{2}$ gives a neighborhood of 1 that contains no points of A distinct from 1. The same is true for the point 2, so we see that A has no cluster points. }
\end{block}
\end{column}
\hfill%
\begin{column}{.48\textwidth}
\begin{figure}[h]
\centering
    \includegraphics[width=5cm]{clusterpoint.jpg}
    \caption{Cluster points}
    \label{}
\end{figure}
\end{column}
\end{columns}
\end{frame}
%\setbeamercolor{frametitle}{bg=red!60,fg=black}
\begin{frame}{}
\fontsize{8pt}{10pt} \selectfont{
\begin{block}{Enumerate}
    \subsection{Enumerate}
\begin{enumerate}[(I)]
     \item For the open interval $A_1 := (0,1)$, every point of the closed interval $[0,1]$ is a cluster point of $A_1$. Note that the points 0,1 are cluster points of $A_1$, but do not belong to $A_1$. All the points of $A_1$ are cluster points of $A_1$.
     \item A finite set has no cluster points.
     \item The infinite set N has no cluster points.
     \item The set $A_4 :={1/n : n \in N}$ has only the point ) as a cluster point. None of the points in $A_4$ is a cluster point of $A_4$.
     \item If $I := [0,1]$, then the set $A_5 := I \cap Q$ consists of all the rational numbers in I. It follows from the Density Theorem 2.4.8 that every point in I is a cluster point of $A_5$. 
\end{enumerate} 
Having made this brief detour, we now return to the concept of the limit of a function at a cluster point of its domain. 
\end{block} 
\setbeamercolor{block title}{bg=pink!40,fg=black}
\begin{block}{Itemize}
\subsection{Itemize}
    \begin{itemize}
        \item $\lim_{x \rightarrow c} f(x)=\textit{L}$.
        \item \textit{Given any $\epsilon$-neighborhood $V_\epsilon(\textit{L}$ of \textit{L}, there exists a $\delta$-neighborhood $V_\delta(c)$ of c such that if $x \neq c$ is any point in $V_\delta(c) \cap A$, then f(x) belongs to $V_\epsilon(\textit{L)}$.}
    \end{itemize}
\end{block} }
\end{frame}
\begin{frame}{\fontfamily{cmtt} \selectfont{\fontsize{10pt}{20pt} \selectfont{THE DEFINITION OF THE LIMIT}}}
\fontsize{8pt}{10pt} \selectfont{
\begin{block}{}
\section{The Definition of the Limit}
 We now state the precise definition of the limit of a function \textit{f} at a point c. It is important to note that in this definition, it is immaterial whether \textit{f} is defined at c or not. In any case, we exclude c from consideration in the determination of the limit.
\subsection{Definition} 
Let $A \subset R$, and let c be a cluster point of A. For a function $\textit{f} : A\rightarrow R$, a real number L is said to be a \textbf{limit of \textit{f} at c} if, given any $\epsilon >0$, there exists a $\delta >0$ such that if $x \in A$ and $0 < |x-c| < \delta$, then $| \textit{f(x)} -\textbf{L}| < \epsilon$.
\textbf{Remarks} 
\end{block} 
\begin{block} {}
    \begin{eqnarray*}
    \prod_{p}\left(1-\frac{1}{p^2}\right)&=&\prod_{p} \frac{1}{1+\frac{1}{p^2}+\frac{1}{p^4}+\cdots}\\
    &=&\left(\prod_{p}\left(1+\frac{1}{p^2}+\frac{1}{p^4}+\cdots\right)\right)^{-1}
\end{eqnarray*}  
\end{block} }
\end{frame}
\begin{frame}{\fontfamily{cmtt} \selectfont{\fontsize{10pt}{20pt} \selectfont{MULTI-LINE EXPRESSIONS}}}
\setbeamercolor{block title}{bg=violet!30,fg=grey!60}
\begin{block}{Equations}
\fontsize{7pt}{2pt} \selectfont{
\section{Multi-line Expressions}
\subsection{Equations}
    1. Let $x=(x_1,\cdots,x_n)$, where the $x_i$ are non-negative real numbers. Set
\begin{equation*}
   M_r(x)=(\frac{x^r_1+x^r_2+\cdots+x^r_n}{n})^{1/r}, \; r\in \mathbf{R}\setminus \{0\} 
\end{equation*}
and
\begin{center}
    $M_0(x)=(x_1x_2\cdots x_n)^{1/n}$.

\end{center}
We call $M_r(x)$ the \textit{rth power mean} of x.
Claim:
\begin{equation*}
      \lim_{r\rightarrow 0}M_r(x)=M_0(x) 
\end{equation*}

    \subsection{Matrix}
        2. Define 
\[
V_n =
\left[
\begin{array}{ccccc}
    1&1&1&\hdots &1 \\
    x_1&x_2&x_3&\hdots&x_n \\
    x^2_1 & x^2_2 & x^2_3&\ldots & x^2_n \\
    \vdots&\vdots&\vdots&\ddots&\vdots\\
    x_1^{n-1}&x_2^{n-1}&x_3^{n-1}&\hdots&x_n^{n-1}
\end{array}
\right]
\]
We call $V_n$ the \textit{Vandermonde matrix} of order n.\\
Claim:
\begin{equation*}
    \det V_n = \prod_{1\leq i \leq j \leq n}(x_j - x_i).
\end{equation*} }
\end{block}
\end{frame}     
\begin{frame}{}
    \begin{block}{}
    \fontsize{8pt}{2pt} \selectfont{ 
    \subsection{Number system}
        \begin{eqnarray*}
   1 +2 &= &3 \\
   4+5+6& = &7+8 \\
   9+10+11+12 &=& 13+14+15\\
   16+17+18+19+20& = &21+22+23+24 \\
   25+26+27+28+29+30 &= &31+32+33+34+35\\ \\
(a+b)^2&=&(a+b)a+(a+b)b \\
    &=&a(a+b)+b(a+b)\\
    &=&a^2+ab+ba+b^2\\
    &=&a^2+ab+ab+b^2\\
    &=&a^2+2ab+b^2
\end{eqnarray*}
\subsection{Trigno.}
\begin{eqnarray*}
    \tan(\alpha+\beta+\gamma)&=&\frac{\tan(\alpha+\beta)+\tan\gamma}{1-\tan(\alpha+\beta)\tan\gamma} \\
    &=&\frac{\frac{\tan\alpha+\tan\beta}{1-\tan\alpha \tan\beta}+\tan\gamma}{1-(\frac{\tan\alpha+\tan\beta}{1-\tan\alpha \tan\beta}\tan\gamma} \\
    &=&\frac{\tan\alpha+\tan\beta+(1-\tan\alpha \tan\beta)\tan\gamma}{1-\tan\alpha \tan\beta-(\tan\alpha+\tan\beta)\tan\gamma}\\
    &=&\frac{\tan\alpha+\tan\beta+\tan\gamma-\tan\alpha \tan\beta \tan\gamma}{1-\tan\alpha \tan\beta-\tan\alpha \tan\gamma-\tan\beta \tan\gamma}
\end{eqnarray*} }
    \end{block}
\end{frame}
\begin{frame}{\fontfamily{cmtt} \selectfont{\fontsize{10pt}{20pt} \selectfont{TABLE}}}
\fontsize{8pt}{10pt} \selectfont {
    \begin{block}{}
        \section{Tables}
        Tables in LaTeX can be created through a combination of the table environment and the tabular environment. The table environment part contains the caption and defines the float for our table, i.e. where in our document the table should be positioned and whether we want it to be displayed centered.
    \begin{center}
    \subsection{Table 1}
\setlength{\arrayrulewidth}{2pt}
    \begin{tabular}{|l|l|l|} \hline
        \multicolumn{3}{|c|}{Country List} \\ \hline
        Country Name or & ISO ALPHA 2  & ISO ALPHA 3 \\
        Area Name & Code & \\ \hline
        Afghanistan & AF & AFG \\ 
        Aland Islands & AX & ALA \\
        Albania & AL & ALB \\
        Algeria & DZ & DZA \\
        American Samoa & AS & ASM \\
        Andorra & AD & AND \\
        Angola & AO & AGO \\ \hline 
    \end{tabular}
\end{center}
    \end{block} }
\end{frame}
\setbeamercolor{block title}{bg=orange!30,}
\begin{frame}
    \begin{block}{\centering Ex.2}
        \subsection{Table 2}
\begin{center}
  \begin{tabular}{||l|l r||} \hline
 gnats & gram & \$13.65 \\ \cline{2-3}
       & each & .01 \\ \hline
       gnu & stuffed & 92.50 \\ \cline{1-1} \cline{3-3}
       emu &   & 33.33 \\ \hline
       armadillo & frozen & 8.99 \\ \hline
\end{tabular}  
\end{center}
\end{block}
\begin{block}{\centering Ex.3}
\subsection{Table 3}
\begin{center}
    \begin{tabular}{|c|c|c|} \hline
    coll & col2 & col3 \\ \hline
    \multirow{2}{*}{Multiple} & cell2 & cell3 \\
    \multirow{2}{*}{row}& cell5 & cell6 \\ 
         & cell8 & cell9 \\ \hline
    \end{tabular}
\end{center}
\end{block}
\end{frame}
\begin{frame}{\fontfamily{cmtt} \selectfont{\fontsize{10pt}{20pt} \selectfont{IMAGES}}}
    \section{Images}
    \begin{block}{}\fontsize{7pt}{6pt} \selectfont {
        LATEX provides several options to handle images and make them look exactly what you need.\\
    Latex can not manage images by itself, so we need to use the graphicx package. To use it, we include the following line in the preamble: \usepackage{graphicx}.
    Plus we can angle the image we want to add in the document. }
    \end{block}
    \begin{figure}
        \centering
        \includegraphics[width=8cm,angle=10]{scenery.jpg}
    \end{figure}
\end{frame}   
\setbeamercolor{frametitle}{bg=red!30,fg=black}
\begin{frame}{\fontfamily{cmtt} \selectfont{\fontsize{10pt}{20pt} \selectfont{BIBLIOGRAPHY}}}
\section{Bibliography}
\begin{block}{}
     \cite{Key1,Key2,Key3}
\begin{thebibliography}{9}
    \bibitem{Key1}{A.Einstein.Zur Elektrodynamik bewegter Korper.(German) [On the electrodynamics of moving bodies].\textit{Annalen der physik},32(10):891-921,1905.doi: http://dx.doi.org/10.1002/andp.19053221004.}
    \bibitem{Key2}{M.Goossens, F.Mittlebach, and A.Samarin. The LaTeX Companion.Addison-Wesley,Reading,Massachusetts,1993.}
    \bibitem{Key3}{D.Knuth.  Knuth:  Computers and typesetting.    URL http://www-cs-faculty.stanford.edu/~uno/abcde.html.}
\end{thebibliography}
\end{block}
\end{frame}
\begin{frame}{}
        \begin{figure}
            \centering
            \includegraphics[width=11cm]{thanks.png}
        \end{figure}
\end{frame}
\end{document}
