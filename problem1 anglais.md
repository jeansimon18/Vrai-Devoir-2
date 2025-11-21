# Problem 1 \[15 Pts\], Data Construction and Summary Analysis

In this question, you will replicate the core inputs of the analysis
from the paper "Expected EPS × Trailing P/E Pricing Without
Discounting." Your task is to gather relevant data, compute key
variables, and provide initial descriptive insights. This process is
meant to mirror the construction of inputs used in the paper's empirical
strategy.

a.  Write code that randomly selects a sample of 50 publicly traded U.S.
    companies from the S&P 500 index and collects the following
    information for each firm: daily (or monthly, if required by the
    paper) stock prices, earnings-per-share (EPS), and trailing
    price-to-earnings (P/E) ratios. Your data should match the frequency
    and time interval used in the original paper. Use WRDS as your data
    source and ensure that your code is easily adaptable to a larger
    sample. \[5 pts\]

b.  Using the data collected in part (a), calculate returns for each
    stock, estimate expected EPS (as defined or implied in the paper),
    and compute the pricing ratio given by trailing P/E. Report your
    code for these transformations clearly. Ensure that any assumptions
    or approximations are explicitly stated. \[5 pts\]

c.  Provide descriptive statistics for each of the following: stock
    price, stock returns, EPS, trailing P/E, and the composite ratio
    Expected EPS × trailing P/E. Generate and clearly label time-series
    plots of each series. In your discussion, highlight any features
    that might be important for the empirical results later in the
    homework --- for example, persistence, outliers, or structural
    breaks. \[5 pts\]
