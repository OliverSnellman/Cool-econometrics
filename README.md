# Cool Econometrics

Personal archive of non-peer-reviewed papers, study materials, simulations, and small programming tools. Some documents were produced while working as a teaching assistant and may build on material prepared by others.

Feel free to use and share these documents.

Oliver Snellman

## Documents

| Document | Theme |
| --- | --- |
| [AD-AS model](AD_AS_model.pdf) | Macroeconomic teaching note |
| [Are Werewolves Vegan?](Are_Werewolves_Vegan.pdf) | Logic, implication, and Hempel's raven |
| [Bounds](Bounds.pdf) | Econometric treatment bounds |
| [Correlation vs Regression](Correlation_vs_Regression.pdf) | Visual intuition for linear association |
| [Ergodicity](Ergodicity.pdf) | Time averages, ensemble averages, and stochastic processes |
| [Friedman's Thermostat](Friedmans_thermostat.pdf) | Monetary policy identification analogy |
| [Hypertrophy](Hypertrophy.pdf) | Training and physiology note |
| [Income and Substitution Effects](Income_and_substitution_effects.pdf) | Microeconomic consumer theory |
| [Introduction to Cryptography](Introduction_to_Cryptography.pdf) | Build-your-own encryption intuition |
| [Introduction to Transformers in Macroeconomics](Introduction_Transformers_macroeconomics.pdf) | Transformer networks for sequential macro data |
| [Limited Dependent Models](Limited%20dependent%20models.pdf) | Binary outcomes, latent variables, and marginal effects |
| [Monetary Policy Model](Monetary_policy_model.pdf) | Three-equation macro model |
| [OLG Model](OLG_model.pdf) | Overlapping generations, pensions, and dynamic efficiency |
| [Panel Data](Panel_data.pdf) | Fixed effects, random effects, and panel structure |
| [Process x](Process_x.pdf) | Heavy tails and non-converging sample means |
| [Regression with Matrices](Regression_with_matrices.pdf) | Matrix notation for OLS |
| [Risk Aversion](Risk_aversion.pdf) | Expected value, utility, and risk premia |
| [Time Series Models](Time_series_models.pdf) | AR, MA, ARMA, and GARCH processes |
| [Tobin's Q](Tobin's%20Q.pdf) | Investment volatility and firm valuation |
| [Yule-Walker Equations](Yule_Walker.pdf) | Estimating autoregressive processes |
| [CV](CV_Snellman.pdf) | Current CV |

## Programming Tools and Templates

| Tool | What it does |
| --- | --- |
| [Expected distance between points](Expected%20distance%20between%20points) | Simulates distances between random points in high-dimensional unit boxes. |
| [Frog jump simulator](Frog%20jump%20simulator) | Simulates a probability puzzle about random jumps across stones. |
| [Game of Life](Game%20of%20Life) | R implementation of Conway's Game of Life, including a glider gun setup. |
| [Monty Hall problem simulator](Monty%20Hall%20problem%20simulator) | Simulates switching and not switching strategies in the Monty Hall problem. |
| [Simulate time series processes](Simulate%20time%20series%20-processes) | Compares AR, MA, ARMA, GARCH, and ARMA-GARCH paths under common shocks. |
| [How to write your Thesis with LaTeX](How%20to%20write%20your%20Thesis%20with%20LaTeX%20-tutorial) | A LaTeX thesis/tutorial template with equations, figures, references, and layout examples. |

## Guided Catalog

### Econometrics and Statistics

#### [Regression with Matrices](Regression_with_matrices.pdf)

A compact introduction to writing regression problems in matrix form. The note shows how systems of equations and matrix notation describe the same linear model.

#### [Correlation vs Regression](Correlation_vs_Regression.pdf)

A visual explanation of how correlation and regression coefficients are related. Correlation $\rho_{X,Y} = \frac{E[(X-\mu_X)(Y-\mu_Y)]}{\sigma_X\sigma_Y}$ measures normalized co-movement; regression $\hat{\beta} = (X'X)^{-1}X'y$ measures the slope of a conditional linear prediction.


#### [Panel Data](Panel_data.pdf)

Teaching notes on cross-sectional, time-series, and panel-data structures. The document introduces the main panel estimators and the practical choice between pooled OLS, random effects, and fixed effects.


#### [Limited Dependent Models](Limited%20dependent%20models.pdf)

Notes on binary outcome models. The central idea is to model a latent index and map it into a probability for outcomes such as yes/no, choice/no choice, or participation/non-participation.


#### [Bounds](Bounds.pdf)

Notes on treatment analysis when point identification is too demanding. The document discusses how assumptions such as monotone instrumental variables, monotone treatment selection, and monotone treatment response can tighten possible effect ranges.


### Time Series and Stochastic Processes

#### [Time Series Models](Time_series_models.pdf)

An introduction to sequentially ordered random variables and the basic processes used to model dependence over time. Covers AR, MA, ARMA, GARCH, and impulse-response intuition.



#### [Yule-Walker Equations](Yule_Walker.pdf)

A note on estimating autoregressive parameters from empirical autocovariances and autocorrelations. Useful as a bridge between time-series theory and actual AR estimation.


#### [Ergodicity](Ergodicity.pdf)

A conceptual note on when the average across many simulated worlds tells us something about one long-run path. The central contrast is between ensemble averages and time averages.

Key idea:

$$
\frac{1}{N}\sum_{i=1}^{N} X_t^{(i)}
\quad \text{versus} \quad
\frac{1}{T}\sum_{t=1}^{T} X_t^{(i)}
$$

#### [Process x](Process_x.pdf)

An exploration of how non-convergence can look like when the issue is not exploding variance.


### Macroeconomics

#### [AD-AS Model](AD_AS_model.pdf)

A step-by-step derivation of the aggregate demand and aggregate supply framework, moving from Keynesian cross logic to IS-LM/TR, New Keynesian demand, and staggered-wage supply.


#### [Monetary Policy Model](Monetary_policy_model.pdf)

A derivation of the three-equation macro model: IS curve, Phillips curve, and monetary-rule curve. The note emphasizes short-run stabilization, central bank behavior, and adaptive expectations.


#### [Friedman's Thermostat](Friedmans_thermostat.pdf)

An explanation of Friedman's thermostat analogy for monetary policy. The note highlights why policy can appear ineffective in naive regressions when the policy instrument is actively stabilizing the target variable.

#### [Tobin's Q](Tobin's%20Q.pdf)

A note on why investment is more volatile than GDP and how Tobin's Q connects firm valuation, expected profits, and the timing of capital investment.


#### [OLG Model](OLG_model.pdf)

Solves the overlapping generations model step by step, then connects the model to dynamic inefficiency and pension-system comparisons between fully funded and pay-as-you-go designs.


#### [Introduction to Transformers in Macroeconomics](Introduction_Transformers_macroeconomics.pdf)

A high-level visual introduction to transformer networks for macroeconomic sequence data. The note connects attention-based machine learning to the special structure of economic time series.

Attention mechanism:

$$
\mathrm{Attention}(Q,K,V)=\mathrm{softmax}\left(\frac{QK'}{\sqrt{d_k}}\right)V
$$

### Microeconomics and Decision Theory

#### [Income and Substitution Effects](Income_and_substitution_effects.pdf)

A teaching note on how households respond when prices, wages, taxes, or relative returns change. The focus is on separating substitution effects from income effects.


#### [Risk Aversion](Risk_aversion.pdf)

Introduces expected value, concave utility, and the idea of a risk premium. The examples explain why a gamble's expected payoff is not enough to determine whether people want to accept it.


### Logic, Computation, and Curiosities

#### [Are Werewolves Vegan?](Are_Werewolves_Vegan.pdf)

A note about material implication, Hempel's raven, and how badly defined propositions can create paradoxes.


#### [Introduction to Cryptography](Introduction_to_Cryptography.pdf)

An introduction to encryption and decryption through the lens of building a simple encryption algorithm.

#### [Hypertrophy](Hypertrophy.pdf)

An introduction to muscle growth.

### Profile

#### [CV](CV_Snellman.pdf)


### Simulations and Small Tools

#### [Simulate time series processes](Simulate%20time%20series%20-processes)

An R simulator for comparing AR, MA, ARMA, GARCH, and ARMA-GARCH processes under shared shocks. Useful for building intuition about how identical innovations propagate through different models.

#### [Game of Life](Game%20of%20Life)

An R implementation of Conway's Game of Life with both random initialization and a glider gun example.

#### [Monty Hall problem simulator](Monty%20Hall%20problem%20simulator)

Simulates repeated Monty Hall games and compares the win rates from switching versus staying.

Key result:

$$
P(\text{win by switching}) = \frac{2}{3}
$$

#### [Frog jump simulator](Frog%20jump%20simulator)

Simulates a river-crossing puzzle where each jump is chosen randomly from the remaining stones. The output shows the distribution and average number of jumps.

#### [Expected distance between points](Expected%20distance%20between%20points)

Approximates the expected distance between two random points in a unit box as dimension increases.

Key object:

$$
E[\|X-Y\|_2], \qquad X,Y \sim U([0,1]^d)
$$

#### [How to write your Thesis with LaTeX](How%20to%20write%20your%20Thesis%20with%20LaTeX%20-tutorial)

A hands-on LaTeX tutorial/template for writing a thesis or paper. Includes examples for document structure, equations, figures, TikZ, hyperlinks, and bibliographic references.

## Note

This reporitory is my personal archive of non-peer-reviewed papers, study materials, side projects and programming tools. Some of the documents were produced as a teaching assistant and they might build upon material prepared by others. 
Feel free to use and share these documents.

Oliver Snellman
18.2.2022