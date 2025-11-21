# Problem 2 \[20 Pts\], Baseline Price Prediction Using EPS × P/E

This question replicates the central empirical claim of the paper: that
stock prices are largely driven by expected EPS and the trailing P/E
ratio, without the need for traditional discounting. You will estimate
and evaluate this model, and compare it against simple alternatives.

a.  Using your dataset from Question 1, estimate a pooled
    cross-sectional regression where the dependent variable is the
    observed price, and the explanatory variable is the product of
    expected EPS and the trailing P/E ratio. Clearly report the
    estimated coefficient, R², and residual summary statistics. How do
    your results compare to those in the referenced paper? \[5 pts\]

b.  Propose and estimate two alternative naive models of the form: (i)
    price on trailing P/E alone, and (ii) price on EPS alone. For each,
    report the R² and compare it to the baseline model. Interpret what
    these results suggest about the joint explanatory power of the two
    inputs. \[5 pts\]

c.  Construct 1-period-ahead forecasts for prices using each of the
    three models. Compute and report the Mean Squared Forecast Error
    (MSFE) for each. Which model forecasts best? How do you know? \[5
    pts\]

d.  Using the model from part (a), produce a time-series plot of actual
    versus predicted prices for one representative firm. Your graph
    should include 95% confidence intervals for the predicted values.
    Comment on whether the model tracks prices well and whether there
    are persistent prediction errors over time. Does the model appear
    overconfident or underconfident? \[5 pts\]
