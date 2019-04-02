# aircraftshapes
Aircraft shapes for use with the [PGF/TikZ](https://www.ctan.org/pkg/pgf?lang=en) LaTeX package. It currently defines shapes for `aircraft side`, `aircraft top`, `quadcopter side`, `quadcopter top`, `helicopter side`, `helicopter top`, `UAM side`, and `UAM top` corresponding to the side and top views of aircraft, quadcopters, helicopters, and urban air mobility vehicles, respectively.

## Example

```latex
\documentclass{article}

\usepackage{tikz}
\usepackage{aircraftshapes}

\begin{document}
	
	\begin{figure}
		\centering
		\begin{tikzpicture}
		\node [aircraft side,fill=black,minimum width=1cm,rotate=10] at (0,0) {};
		\node [aircraft side,fill=black,minimum width=1cm,xscale=-1] at (5,1) {}; 
		\end{tikzpicture}
		\caption{Aircraft side.}
	\end{figure}
	
	\begin{figure}
		\centering
		\begin{tikzpicture}
		\node [aircraft top,fill=black,minimum width=1cm] at (0,0) {};
		\node [aircraft top,fill=black,minimum width=1cm,xscale=-1] at (5,1) {}; 
		\end{tikzpicture}
		\caption{Aircraft top.}
	\end{figure}

	\begin{figure}
		\centering
		\begin{tikzpicture}
		\node [quadcopter side,fill=white,draw=black,minimum width=1cm] at (0,0) {};
		\node [quadcopter side,fill=white,draw=black,minimum width=1cm,rotate=20] at (5,1) {}; 
		\end{tikzpicture}
		\caption{Quadcopter side.}
	\end{figure}

	\begin{figure}
		\centering
		\begin{tikzpicture}
		\node [quadcopter top,fill=white,draw=black,minimum width=1cm,scale=0.5] at (0,0) {};
		\node [quadcopter top,fill=white,draw=black,minimum width=1cm,rotate=20,scale=0.5] at (5,1) {}; 
		\end{tikzpicture}
		\caption{Quadcopter top.}
	\end{figure}

	\begin{figure}
		\centering
		\begin{tikzpicture}
		\node [helicopter side,fill=black,draw=black,minimum width=1cm,scale=0.4] at (0,0) {};
		\node [helicopter side,fill=black,draw=black,minimum width=1cm,rotate=20,scale=0.4,xscale=-1] at (5,1) {}; 
		\end{tikzpicture}
		\caption{Helicopter side.}
	\end{figure}

	\begin{figure}
		\centering
		\begin{tikzpicture}
		\node [helicopter top,fill=black,draw=black,minimum width=1cm,scale=0.6] at (0,0) {};
		\node [helicopter top,fill=black,draw=black,minimum width=1cm,rotate=20,scale=0.6] at (5,1) {}; 
		\end{tikzpicture}
		\caption{Helicopter top.}
	\end{figure}

	\begin{figure}
		\centering
		\begin{tikzpicture}
		\node [UAM side,fill=white,draw=black,minimum width=2cm] at (0,0) {};
		\node [UAM side,fill=white,draw=black,minimum width=2cm,rotate=20,xscale=-1] at (5,1) {}; 
		\end{tikzpicture}
		\caption{Urban Air Mobility Vehicle side.}
	\end{figure}

	\begin{figure}
		\centering
		\begin{tikzpicture}
		\node [UAM top,fill=black,draw=black,minimum width=1cm,scale=0.5] at (0,0) {};
		\node [UAM top,fill=black,draw=black,minimum width=1cm,rotate=20,scale=0.5] at (5,1) {}; 
		\end{tikzpicture}
		\caption{Urban Air Mobility Vehicle top.}
	\end{figure}


\end{document}
```
