\documentclass[t]{beamer}

% --- Packages ---
\usepackage[utf8]{inputenc}
\usepackage{xcolor}
\usepackage{hyperref}
\usepackage{tikz}
\usepackage{booktabs}
\usepackage{natbib}
\usepackage{graphicx}
% --- Theme and Color Setup ---
\usetheme{Madrid}

% Define custom blue color
\definecolor{MyBlue}{RGB}{0,102,204}

% Apply blue color to the structure
\usecolortheme[named=MyBlue]{structure}

% Footer colors
\setbeamercolor{palette primary}{bg=MyBlue,fg=white}
\setbeamercolor{palette secondary}{bg=MyBlue!80!black,fg=white}
\setbeamercolor{palette tertiary}{bg=MyBlue!60!black,fg=white}

% Caption font
\setbeamerfont{caption}{size=\footnotesize}

% --- CONFIGURATION FOR FIRST & LAST PAGE ---
\newcommand{\FirstLastPageLayout}{}

% --- Presentation Information ---
\title[Mathematics for Computing]{Mathematics for Computing}
\subtitle{Assignment}
\author{DILNA P}

\institute[]{
M.Tech in Computer Science and Engineering\\
Specialization in Data Science and Artificial Intelligence\\[0.3cm]
Department of Computer Science, CUSAT
}

\date{\today}

\begin{document}

% --- Slide 1: Title Page ---
\begin{frame}
    \titlepage
\end{frame}
% --- Slide: Contents ---
\begin{frame}{Contents}
\small

\begin{enumerate}
    \item Introduction to Statistics
    \item Types of Statistics
    \item Government Statistical Departments
    \item Types of Data
    \item Measures of Central Tendency
    \item Measures of Dispersion
    \item Measures of Position
    \item Interquartile Range (IQR)
    \item Outliers
    \item Skewness
    \item Kurtosis
    \item Module 3
\end{enumerate}

\end{frame}
% --- Slide: Introduction to Statistics ---
\begin{frame}{Introduction to Statistics}
\small

Statistics is the science of \textbf{collecting, organizing,
analyzing, interpreting, and presenting data}. It helps us
understand large amounts of information and make better decisions.

\vspace{0.15cm}

For example, statistics can be used to study \textbf{population,
education, employment, health, business, and the economy}.
Governments and organizations collect data, organize it using
tables and graphs, analyze it using statistical methods, and use
the results for planning and decision-making.

\vspace{0.2cm}

\textbf{In simple words:}

\[
\text{Data Collection}
\rightarrow
\text{Organization}
\rightarrow
\text{Analysis}
\rightarrow
\text{Interpretation}
\rightarrow
\text{Decision Making}
\]

\vspace{0.15cm}

Thus, statistics helps us convert \textbf{raw data into useful
information}.

\end{frame}
% --- Slide: Types of Statistics ---
\begin{frame}{Types of Statistics}
\small

Statistics is mainly divided into two types:

\vspace{0.3cm}

\begin{center}
\textbf{Statistics}

\vspace{0.2cm}

\begin{tabular}{ccc}
& $\downarrow$ & \\[-0.1cm]
\textbf{Descriptive Statistics} & & \textbf{Inferential Statistics} \\[0.1cm]
\text{Summarizes Data} & & \text{Makes Conclusions}
\end{tabular}
\end{center}

\vspace{0.25cm}

\textbf{1. Descriptive Statistics}

Used to collect, organize, summarize, and present data.

\textbf{Examples:} Mean, Median, Mode, Variance, Tables, Graphs,
and Histograms.

\vspace{0.15cm}

\textbf{2. Inferential Statistics}

Used to make conclusions or predictions about a population
using a sample.

\textbf{Examples:} Sampling, Confidence Intervals, Hypothesis
Testing, Estimation, and Prediction.

\end{frame}
% --- Slide: Department of Economics and Statistics, Kerala ---
\begin{frame}{Department of Economics and Statistics, Kerala}
\small

\begin{itemize}
    \item The \textbf{Department of Economics and Statistics (DES)}
    is the nodal agency for official statistics in Kerala.

    \item Collects, compiles, analyzes, interprets, and publishes
    statistical information.

    \item Collects data related to:
    \begin{itemize}
        \item Agriculture,Industry,Employment,Prices ,Population
    \end{itemize}

    \item Prepares important economic indicators such as:
    \begin{itemize}
        \item Gross State Domestic Product (GSDP)
        \item Per-capita Income
    \end{itemize}

    \item Collects farm, wholesale, and retail price data and prepares
    price indices.

    \item Conducts surveys and studies for government planning,
    policy-making, and evaluation of development programmes.

    \item Publishes statistical reports, databases, and analytical
    information for government agencies, researchers, and the public.
\end{itemize}

\end{frame}
% --- Slide: MoSPI, Government of India ---
\begin{frame}{MoSPI, Government of India}
\small

\begin{itemize}
    \item \textbf{MoSPI} coordinates India's national statistical system
    and statistical activities.

    \item Works with Central Ministries, State Governments, and
    Union Territories.

    \item Sets standards for data collection, processing, analysis,
    and dissemination.

    \item Prepares important national statistics, including
    National Accounts and national income estimates.

    \item Conducts surveys on employment, household consumption,
    enterprises, and other socio-economic areas.

    \item Develops indicators for monitoring the
    \textbf{Sustainable Development Goals (SDGs)}.

    \item Monitors major government projects and programmes,
    including \textbf{MPLADS}.

    \item Supports planning, policy-making, and national development.
\end{itemize}

\end{frame}

% --- Slide 1: Univariate Data ---
\begin{frame}{Types of Data-Univariate Data}
\small

\textbf{Definition:}

Univariate data contains information about only \textbf{one variable}.

\vspace{0.2cm}

\textbf{Example: Student Marks}

\[
X = \{60, 70, 75, 80, 90\}
\]

Here, only one variable, \textbf{marks}, is studied.

\vspace{0.2cm}

\textbf{Application:}

Univariate data can be analyzed using measures such as:

\begin{itemize}
    \item Mean
    \item Median
    \item Mode
    \item Variance
    \item Histogram
\end{itemize}

\end{frame}


% --- Slide 2: Bivariate Data ---
\begin{frame}{Types of Data-Bivariate Data}
\small

\textbf{Definition:}

Bivariate data contains information about \textbf{two variables}.
It is often used to study the relationship between the variables.

\vspace{0.2cm}

\textbf{Example: Height and Weight}

\[
(X,Y)=\{(160,55),(165,60),(170,65)\}
\]

where:

\begin{itemize}
    \item \(X\) = Height
    \item \(Y\) = Weight
\end{itemize}

\vspace{0.2cm}

\textbf{Application:}

Bivariate data can be used to study relationships using:

\begin{itemize}
    \item Scatter plots
    \item Correlation
    \item Regression
\end{itemize}

\end{frame}


% --- Slide 3: Multivariate Data ---
\begin{frame}{Types of Data-Multivariate Data}
\small

\textbf{Definition:}

Multivariate data contains information about \textbf{more than two
variables}.

\vspace{0.2cm}

\textbf{Example: Student Information}

\[
(\text{Age},\text{Height},\text{Weight},\text{Marks})
\]

Here, several variables are studied together.

\vspace{0.2cm}

\textbf{Application:}

Multivariate data analysis is useful for studying complex data
where many variables influence each other.

\begin{itemize}
    \item Machine Learning
    \item Data Science
    \item Prediction and Classification
\end{itemize}

\end{frame}

% --- Slide: Measures of Central Tendency ---
\begin{frame}{Measures of Central Tendency}
\small

\textbf{Definition:}

Measures of central tendency are statistical measures used to find the
\textbf{central or typical value} of a dataset.

\vspace{0.15cm}

\textbf{The three main measures are:}

\begin{itemize}
    \item \textbf{Mean:} The average value of the data.
    \item \textbf{Median:} The middle value when data is arranged in order.
    \item \textbf{Mode:} The value that occurs most frequently.
\end{itemize}

\vspace{0.1cm}

\textbf{Example:}

\[
2,\;4,\;4,\;6,\;8
\]

\[
\text{Mean}=\frac{2+4+4+6+8}{5}=4.8
\qquad
\text{Median}=4
\qquad
\text{Mode}=4
\]

\vspace{0.1cm}

\textbf{In simple words:} These measures help us find a single value
that represents the center of the data.

\end{frame}

% --- Slide: Measures of Dispersion ---
\begin{frame}{Measures of Dispersion}
\small

\textbf{Definition:}

Measures of dispersion show how \textbf{spread out or scattered}
the values are in a dataset.

\vspace{0.15cm}

\textbf{Main Measures of Dispersion:}

\begin{itemize}
    \item \textbf{Range:} Difference between the largest and smallest values.
    \[
    \text{Range}=\text{Maximum}-\text{Minimum}
    \]

    \item \textbf{Variance:} Measures how far the data values are
    spread from the mean.

    \item \textbf{Standard Deviation:} Shows the amount by which
    data values differ from the mean.

    \item \textbf{Interquartile Range (IQR):} Measures the spread of
    the middle \(50\%\) of the data.
    \[
    \text{IQR}=Q_3-Q_1
    \]
\end{itemize}

\vspace{0.1cm}

\textbf{Example:}
\[
2,\;4,\;6,\;8,\;10
\]
\[
\text{Range}=10-2=8
\]
\end{frame}

% --- Slide: Measures of Position ---
\begin{frame}{Measures of Position}
\small

\textbf{Definition:}

Measures of position show the \textbf{relative location of a value}
within a dataset.

\vspace{0.15cm}

\textbf{Main Measures:}

\begin{itemize}
    \item \textbf{Quartiles:} Divide the data into four equal parts.
    
    \item \textbf{Deciles:} Divide the data into ten equal parts.
    
    \item \textbf{Percentiles:} Divide the data into one hundred
    equal parts.
\end{itemize}

\vspace{0.15cm}

\textbf{Example:}

If a student is in the \(90^{\text{th}}\) percentile, the student's
score is higher than approximately \(90\%\) of the scores.

\vspace{0.15cm}

\textbf{Application:}

Measures of position are used to compare the relative standing of
values in a dataset.

\end{frame}

% --- Slide: Interquartile Range (IQR) ---
\begin{frame}{Interquartile Range (IQR)}
\small

\textbf{Definition:}

The \textbf{Interquartile Range (IQR)} measures the spread of the
\textbf{middle 50\% of the data}.

\vspace{0.15cm}

\textbf{Formula:}
\[
\text{IQR}=Q_3-Q_1
\]
where:
\begin{itemize}
    \item \(Q_1\) = First Quartile (25th percentile)
    \item \(Q_3\) = Third Quartile (75th percentile)
\end{itemize}

\vspace{0.1cm}

\textbf{Example:}

Consider the ordered data:
\[
2,\;4,\;6,\;8,\;10,\;12,\;14,\;16
\]
\[
Q_1=5,\qquad Q_3=13
\]
Therefore:
\[
\text{IQR}=Q_3-Q_1=13-5=8
\]
\vspace{0.5cm}
\textbf{In simple words:} IQR tells us how widely the middle half
of the data is spread.

\end{frame}

% --- Slide: Outliers ---
\begin{frame}{Outliers}
\small

\textbf{Definition:}

An \textbf{outlier} is a data value that is very different from most
of the other values in a dataset.

\vspace{0.15cm}

\textbf{IQR Method for Detecting Outliers:}
\[
\text{IQR}=Q_3-Q_1
\]
\[
\text{Lower Limit}=Q_1-1.5(\text{IQR})
\]
\[
\text{Upper Limit}=Q_3+1.5(\text{IQR})
\]
Any value:
\[
< \text{Lower Limit}
\qquad \text{or} \qquad
> \text{Upper Limit}
\]
is considered an \textbf{outlier}.
\vspace{0.5cm}
\textbf{Example:}
\[
2,\;4,\;6,\;8,\;10,\;12,\;14,\;30
\]
The value \(\mathbf{30}\) is far from most other values and may be
considered an outlier.

\vspace{0.1cm}

\textbf{In simple words:} An outlier is an unusual value that is far
away from most of the data.
\end{frame}

% --- Slide: Skewness ---
\begin{frame}{Skewness}
\small

\textbf{Definition:}

Skewness is a measure of the \textbf{asymmetry} of a data distribution.

\vspace{0.15cm}

\textbf{Types of Skewness:}

\begin{itemize}
    \item \textbf{Zero Skewness:} The distribution is symmetric.
    
    \item \textbf{Positive Skewness:} The distribution has a longer
    tail on the right side.
    
    \item \textbf{Negative Skewness:} The distribution has a longer
    tail on the left side.
\end{itemize}

\vspace{0.15cm}

\textbf{Relationship between Mean, Median and Mode:}
\[
\text{Negative Skew: Mean < Median < Mode}
\]
\[
\text{Symmetric: Mean = Median = Mode}
\]
\[
\text{Positive Skew: Mode < Median < Mean}
\]
\vspace{0.1cm}

\textbf{Application:} Skewness helps us understand the shape and
asymmetry of data.

\end{frame}

% --- Slide: Kurtosis ---
\begin{frame}{Kurtosis}
\small

\textbf{Definition:}

Kurtosis is a measure that describes the \textbf{shape, peakedness,
and tail behavior} of a data distribution.

\vspace{0.15cm}

\textbf{Types of Kurtosis:}

\begin{itemize}
    \item \textbf{Mesokurtic:} A distribution with normal or moderate
    peakedness.

    \item \textbf{Leptokurtic:} A distribution with a sharper peak
    and heavier tails.

    \item \textbf{Platykurtic:} A distribution with a flatter peak
    and lighter tails.
\end{itemize}

\vspace{0.15cm}

\textbf{Kurtosis Value:}

\[
\text{Kurtosis} = 3
\quad \Rightarrow \quad
\text{Mesokurtic}
\]
\[
\text{Kurtosis} > 3
\quad \Rightarrow \quad
\text{Leptokurtic}
\]
\[
\text{Kurtosis} < 3
\quad \Rightarrow \quad
\text{Platykurtic}
\]

\vspace{0.1cm}

\textbf{Application:} Kurtosis helps us understand the shape and
tail behavior of a data distribution.

\end{frame}
\begin{frame}{Graphical Representation of Skewness and Kurtosis}

\centering

\includegraphics[width=\textwidth]{ChatGPT Image Sep 5, 2026, 08_39_47 PM.png}

\end{frame}

% --- Slide 4: Histogram ---
\begin{frame}{Histogram}

A histogram is a graphical representation used to understand the
distribution of numerical data.

\begin{itemize}
    \item Numerical data is divided into intervals called \textbf{bins}.
    
    \item The height of each bar represents the frequency of observations.
    
    \item The bars are placed next to each other without gaps.
    
    \item For unequal class intervals, frequency density is calculated as:
\end{itemize}

\[
\text{Frequency Density}
=
\frac{\text{Frequency}}{\text{Class Width}}
\]

\begin{itemize}
    \item It helps us understand the shape, center, and spread of data.
\end{itemize}

\end{frame}

% --- Slide 5: Sample Mean ---
\begin{frame}{Sample Mean}

\textbf{Definition}

Sample mean is the average value of all observations in a sample.
It represents the central value of the given data.

\vspace{0.3cm}

\textbf{Equation}
\[
\bar{x}=\frac{1}{n}\sum_{i=1}^{n}x_i
\]
where:
\begin{itemize}
    \item \(x_i\) = individual observation
    \item \(n\) = total number of observations
    \item \(\bar{x}\) = sample mean
\end{itemize}

\textbf{Example}
For the data \(2,4,6,8\):
\[
\bar{x}=\frac{2+4+6+8}{4}=5
\]

\textbf{Application:} Used in data analysis to find the average value of a dataset.
\end{frame}


% --- Slide 6: Sample Variance ---
\begin{frame}{Sample Variance}
\small

\textbf{Definition:} Sample variance measures how much data values
are spread around the sample mean.

\vspace{0.15cm}

\textbf{Equation:}

\[
s^2=\frac{1}{n-1}\sum_{i=1}^{n}(x_i-\bar{x})^2
\]

where \(x_i\) is an observation, \(\bar{x}\) is the mean,
and \(n\) is the sample size.

\vspace{0.15cm}

\textbf{Example:}

For \(2,4,6\), where \(\bar{x}=4\):

\[
s^2=\frac{(2-4)^2+(4-4)^2+(6-4)^2}{3-1}=4
\]

\textbf{Application:} Used to measure the variability or consistency
of data.

\end{frame}

% --- Slide 7: Order Statistics ---
\begin{frame}{Order Statistics}
\small

\textbf{Definition:} Order statistics are the observations of a sample
arranged in ascending or descending order.

\vspace{0.15cm}

\textbf{Notation:}

For a sample \(X_1,X_2,\ldots,X_n\), after arranging the values:

\[
X_{(1)} \leq X_{(2)} \leq \cdots \leq X_{(n)}
\]

where \(X_{(1)}\) is the smallest value and \(X_{(n)}\) is the
largest value.

\vspace{0.15cm}

\textbf{Example:}

For the data \(5,2,8,1,6\):

\[
1,2,5,6,8
\]

Thus,

\[
X_{(1)}=1,\qquad X_{(5)}=8
\]

\textbf{Application:} Used to find the minimum, maximum, median,
percentiles, and other ranked values in data.

\end{frame}

% --- Slide 8: Sample Covariance ---
\begin{frame}{Sample Covariance}
\small

\textbf{Definition:}

Sample covariance measures how two variables change together.

\begin{itemize}
    \item Positive covariance: Both variables tend to increase or decrease together.
    \item Negative covariance: One variable tends to increase while the other decreases.
    \item Zero covariance: No linear relationship is indicated.
\end{itemize}

\textbf{Equation:}

\[
s_{XY}=
\frac{1}{n-1}
\sum_{i=1}^{n}
(X_i-\bar{X})(Y_i-\bar{Y})
\]

where \(X_i\) and \(Y_i\) are observations, and
\(\bar{X}\) and \(\bar{Y}\) are their sample means.

\textbf{Application:} Used to study relationships between variables,
such as study hours and examination marks.

\end{frame}

% --- Slide 9: Sample Covariance Example ---
\begin{frame}{Sample Covariance: Example}
\small

Consider two students:

\[
X=(1,3), \qquad Y=(2,6)
\]

\textbf{Step 1: Find the means}

\[
\bar{X}=\frac{1+3}{2}=2,
\qquad
\bar{Y}=\frac{2+6}{2}=4
\]

\textbf{Step 2: Calculate covariance}

\[
s_{XY}
=
\frac{(1-2)(2-4)+(3-2)(6-4)}{2-1}
\]

\[
=
\frac{2+2}{1}=4
\]

\textbf{Result:} Covariance is positive, so \(X\) and \(Y\)
increase together.

\end{frame}

% --- Slide 10: Sample Covariance Matrix ---
\begin{frame}{Sample Covariance Matrix}
\small

\textbf{Definition:}

A sample covariance matrix shows the variance and covariance
between two or more variables.

\vspace{0.2cm}

\textbf{Equation:}

For two variables \(X\) and \(Y\):

\[
S=
\begin{bmatrix}
s_X^2 & s_{XY}\\
s_{XY} & s_Y^2
\end{bmatrix}
\]

where:

\begin{itemize}
    \item \(s_X^2\) = variance of \(X\)
    \item \(s_Y^2\) = variance of \(Y\)
    \item \(s_{XY}\) = covariance between \(X\) and \(Y\)
\end{itemize}

\textbf{Application:}

Used in machine learning and data analysis to understand relationships
between multiple variables.

\end{frame}
% --- Slide 11: Sample Covariance Matrix Example ---
\begin{frame}{Sample Covariance Matrix: Example}
\small

Consider:

\[
X=(1,3), \qquad Y=(2,6)
\]

From the previous calculations:

\[
s_X^2=2,\qquad s_Y^2=8,\qquad s_{XY}=4
\]

Therefore, the sample covariance matrix is:

\[
S=
\begin{bmatrix}
2 & 4\\
4 & 8
\end{bmatrix}
\]

\textbf{Interpretation:}

\begin{itemize}
    \item Diagonal values represent variances.
    \item Off-diagonal values represent covariance.
    \item Positive covariance shows that \(X\) and \(Y\) tend to increase together.
\end{itemize}

\end{frame}
% --- Slide: Frequentist Statistics ---
\begin{frame}{Frequentist Statistics}
\small

\textbf{Definition:}

Frequentist statistics interprets probability as the long-run
frequency of an event after repeated experiments.

\vspace{0.15cm}

\textbf{Main Idea:}

\begin{itemize}
    \item Parameters are fixed but unknown.
    \item Probability is estimated using repeated observations.
\end{itemize}

\textbf{Equation:}

\[
P(A) \approx
\frac{\text{Number of times event } A \text{ occurs}}
{\text{Total number of trials}}
\]

\textbf{Example:}

A coin is tossed \(100\) times and heads occurs \(55\) times:

\[
P(\text{Heads})=\frac{55}{100}=0.55
\]

\textbf{Applications:} Hypothesis testing, confidence intervals,
scientific experiments, and data analysis.

\end{frame}

% --- Slide: Sampling ---
\begin{frame}{Sampling}
\small

\textbf{Definition:}

Sampling is the process of selecting a smaller group, called a
\textbf{sample}, from a larger group, called a \textbf{population}.

\vspace{0.2cm}

\textbf{Types of Sampling:}

\begin{itemize}
    \item \textbf{Random Sampling:} Every member has an equal chance of being selected.
    
    \item \textbf{Systematic Sampling:} Every \(k\)-th member is selected from the population.
    
    \item \textbf{Stratified Sampling:} The population is divided into groups, and samples are selected from each group.
\end{itemize}

\vspace{0.15cm}

\textbf{Application:} Sampling saves time, cost, and effort when
studying a large population.

\end{frame}

% --- Slide: Sampling Example ---
\begin{frame}{Sampling: Example}
\small

\textbf{Example: Student Survey}

Suppose a university has \(10,000\) students, and a researcher
randomly selects \(500\) students for a survey.

\vspace{0.15cm}

\textbf{Sampling Fraction:}

\[
f=\frac{n}{N}
\]

where:

\[
n=\text{Sample Size}, \qquad N=\text{Population Size}
\]

For this example:

\[
f=\frac{500}{10,000}=0.05=5\%
\]

\textbf{Conclusion:}

The researcher studies \(5\%\) of the population and uses the
sample results to make conclusions about the entire population.

\end{frame}

% --- Slide: IID Sampling ---
\begin{frame}{IID Sampling}
\small

\textbf{Definition:}

IID stands for \textbf{Independent and Identically Distributed}.
It means that each observation is generated independently from
the same probability distribution.

\vspace{0.15cm}

\textbf{Mathematical Representation:}

\[
X_1,X_2,\ldots,X_n \overset{\text{iid}}{\sim} P
\]

where \(P\) represents the common probability distribution.

\vspace{0.15cm}

\textbf{Main Properties:}

\begin{itemize}
    \item \textbf{Independent:} One observation does not affect another.
    \item \textbf{Identically Distributed:} All observations follow the
    same probability distribution.
\end{itemize}

\textbf{Application:}

IID sampling is widely used in statistical estimation and machine
learning to analyze data and estimate population parameters.

\end{frame}
% --- Slide: IID Sampling Example ---
\begin{frame}{IID Sampling: Example}
\small

\textbf{Example: Rolling a Fair Die}

Suppose a fair die is rolled \(5\) times:

\[
X_1=2,\quad X_2=5,\quad X_3=2,\quad X_4=4,\quad X_5=2
\]

The number \(2\) appears more than once, which is possible because
each roll is independent.

\vspace{0.15cm}

\textbf{Independent:}

The result of one roll does not affect the next roll.

\vspace{0.1cm}

\textbf{Identically Distributed:}

Each roll has the same probability distribution:

\[
P(X_i=k)=\frac{1}{6},
\qquad k=1,2,\ldots,6
\]

Therefore:

\[
X_1,X_2,\ldots,X_5
\overset{\text{iid}}{\sim}
\text{Uniform}\{1,2,3,4,5,6\}
\]

\end{frame}

% --- Slide: Mean Square Error ---
\begin{frame}{Mean Square Error}
\small

\textbf{Definition:}

Mean Square Error (MSE) measures the average squared difference
between an estimated value and the true value.

\vspace{0.15cm}

\textbf{Equation:}

\[
\mathrm{MSE}(\hat{\theta})
=
E\left[(\hat{\theta}-\theta)^2\right]
\]

where:

\begin{itemize}
    \item \(\theta\) = true parameter
    \item \(\hat{\theta}\) = estimated parameter
    \item \(E\) = expected value
\end{itemize}

\textbf{Application:}

MSE is used to evaluate the accuracy of estimators and prediction
models. A smaller MSE indicates a more accurate estimate.

\end{frame}
% --- Slide: Mean Square Error Example ---
\begin{frame}{Mean Square Error: Example}
\small

Suppose the true values and estimated values are:

\[
\text{True Values: } 2,\ 4,\ 6
\]

\[
\text{Estimated Values: } 3,\ 5,\ 5
\]

\textbf{Step 1: Find the squared errors}

\[
(2-3)^2=1,\qquad
(4-5)^2=1,\qquad
(6-5)^2=1
\]

\textbf{Step 2: Calculate MSE}

\[
\mathrm{MSE}
=
\frac{1}{n}
\sum_{i=1}^{n}
(y_i-\hat{y}_i)^2
\]

\[
\mathrm{MSE}
=
\frac{1+1+1}{3}=1
\]

\textbf{Result:} The Mean Square Error is \(\boxed{1}\).

\end{frame}
% --- Slide: Consistency ---
\begin{frame}{Consistency}
\small

\textbf{Definition:}

An estimator is called \textbf{consistent} if its estimated value gets
closer to the true parameter as the sample size increases.

\vspace{0.15cm}

\textbf{Mathematical Condition:}

\[
\hat{\theta}_n \xrightarrow{P} \theta
\quad \text{as } n \rightarrow \infty
\]

This means that the probability of the estimator being close to the
true parameter approaches \(1\) as the sample size increases.

\vspace{0.15cm}

\textbf{Simple Idea:}

\[
\text{More Data} \quad \Longrightarrow \quad
\text{Better Estimate of the True Value}
\]

\textbf{Application:}

Consistency is used to evaluate whether a statistical estimator
becomes more accurate when more data is collected.

\end{frame}

% --- Slide: Confidence Intervals ---
\begin{frame}{Confidence Intervals}
\small

\textbf{Definition:}
A confidence interval is a range of values calculated from sample data that is likely to contain the true population parameter.


A \(1-\alpha\) confidence interval \(I\) for an unknown parameter
\(\gamma \in \mathbb{R}\) satisfies:

\[
P(\gamma \in I) \geq 1-\alpha,
\qquad 0<\alpha<1
\]

\vspace{0.15cm}

\textbf{For the Mean of an IID Sequence:}

If the variance satisfies:

\[
\sigma^2 \leq b^2
\]

then a confidence interval is:

\[
I_n =
\left[
\overline{Y}_n-\frac{b}{\sqrt{\alpha n}},
\;
\overline{Y}_n+\frac{b}{\sqrt{\alpha n}}
\right]
\]

\vspace{0.1cm}

\textbf{Key Point:}

A confidence interval gives a range rather than a single value,
allowing us to quantify uncertainty when estimating a parameter
from finite data.

\end{frame}

% --- Slide: Parametric Model Estimation ---
\begin{frame}{Parametric Model Estimation}
\small

\textbf{Definition:}

Parametric model estimation assumes that the data follows a model
with a fixed number of unknown parameters. These parameters are
estimated using the available sample data.

\vspace{0.15cm}

\textbf{General Form:}
\[
Y \sim P_{\theta}
\]
where:
\begin{itemize}
    \item \(Y\) = observed data
    \item \(P_{\theta}\) = probability model
    \item \(\theta\) = unknown parameter to be estimated
\end{itemize}

\textbf{Example:}

For a normal distribution:
\[
Y \sim \mathcal{N}(\mu,\sigma^2)
\]
The unknown parameters \(\mu\) and \(\sigma^2\) are estimated from
the sample data.

\textbf{Application:} Used when the underlying probability model of
the data is known or assumed.

\end{frame}
% --- Slide: Non-Parametric Model Estimation ---
\begin{frame}{Non-Parametric Model Estimation}
\small

\textbf{Definition:}

Non-parametric model estimation does not assume that the data follows
a specific probability distribution with a fixed set of parameters.

\vspace{0.15cm}

Instead, the model is estimated directly from the available data.

\vspace{0.15cm}

\textbf{General Idea:}

\[
\text{Data}
\quad \longrightarrow \quad
\text{Estimate the Model}
\]

\vspace{0.15cm}

\textbf{Example:}

A histogram can be used to estimate the distribution of data without
assuming that the data follows a normal or any other specific
distribution.

\vspace{0.15cm}

\textbf{Application:}

Non-parametric methods are useful when the underlying distribution of
the data is unknown or difficult to assume.

\end{frame}
\end{document}

