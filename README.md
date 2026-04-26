# Cool Econometrics

This reporitory is my personal archive of non-peer-reviewed papers, study materials, side projects and programming tools. Some of the documents were produced as a teaching assistant and they might build upon material prepared by others. 
Feel free to use and share these documents.

Oliver Snellman
18.2.2022


## Catalog

### Econometrics and Statistics

#### [Regression with Matrices](Regression_with_matrices.pdf)

Introduction to writing regression problems in matrix form. The note shows how systems of equations and matrix notation describe the same linear model.

#### [Correlation vs Regression](Correlation_vs_Regression.pdf)

Correlation and regression coefficients both describe a certain type of relation between two variables. Here I provide a visual intuition on how they differ.


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

Walkthrough (advanced) of equations, which are used to estimate the autoregressive parameters and error variances of an AR(p) process, based on the empirical autocovariances and autocorrelations.

#### [Ergodicity](Ergodicity.pdf)

A notebook showing how the average over different outcomes of an activity can give you false information on what to expect if you take part in the activity yourself.

A system is ergodic, when:

$$
\frac{1}{N}\sum_{i=1}^{N} X_i(t)
\quad = \quad
\frac{1}{T}\sum_{t=1}^{T} X_t(i)
$$

#### [Process x](Process_x.pdf)

An example of a process with finite variance but non-converging mean.


### Macroeconomics

#### [AD-AS Model](AD_AS_model.pdf)

The AD-AS model is a pedagogical tool, which uses graphical analysis to build qualitative intuitions about the macro-economy. In this document I show how to derive the model step by step, starting from the Keynes Cross model to get to the IS-LM/TR model, from which the demand side AD curve arises from. I also derive the microfounded New Keynesian AD relation from household's problem. Finally, I derive the supply side AS curve using staggered wage setting.

#### [Monetary Policy Model](Monetary_policy_model.pdf)

In this document I derive another version of the AD-AS model, which focuses on the role of the Central Bank (CB) and monetary policy on stabilizing the economy over the short run business cycle. The model consists of the IS curve describing the demand side, Phillips curve for the supply side and the MR curve for the policymaker (CB). Households and wage setters have adaptive expectations, whereas the CB has rational expectations.

#### [Friedman's Thermostat](Friedmans_thermostat.pdf)

A visual intuition to the endogeneity problem, with a practical example.

#### [Tobin's Q](Tobin's%20Q.pdf)

Short recap of the model of investments.

#### [OLG Model](OLG_model.pdf)

In these notes I first analytically solve the heterogenous agent OLG model step by step, followed by a short conversation about dynamic inefficiency, and finish by comparing the efficiency of the two common pension systems, fully funded and pay as you go.

#### [Introduction to Transformers in Macroeconomics](Introduction_Transformers_macroeconomics.pdf)

Non-technical overview of my PhD dissertation, emphasizing visual intuition on using transformer networks for macroeconomic sequence data. The material shows how to use attention-based machine learning to estimate and interpret latent structures form small time series datasets.

Attention mechanism:

$$
\mathrm{Attention}(Q,K,V)=\mathrm{softmax}\left(\frac{QK'}{\sqrt{d_k}}\right)V
$$

### Microeconomics and Decision Theory

#### [Income and Substitution Effects](Income_and_substitution_effects.pdf)

A teaching note on how does changes in income or prices affect consumption decisions?


#### [Risk Aversion](Risk_aversion.pdf)

Introduces expected value, concave utility, and the idea of a risk premium. The examples explain why a gamble's expected payoff is not enough to determine whether people want to accept it or not.


### Logic, Computation, and Curiosities

#### [Are Werewolves Vegan?](Are_Werewolves_Vegan.pdf)

I first introduce the concept of implication in propositional logic, then present a puzzling consequence of it called Hempel’s paradox and provide an intuition for why it is not really a paradox. Lastly, I point attention to a situation where the paradox does arise, due to poorly defined propositions.


#### [Introduction to Cryptography](Introduction_to_Cryptography.pdf)

In this document I walk through visually the process of encrypting a message with a simple example. Why is it not possible to "crack the code" of modern encryption algorithms? Because they use pseudo-randomness to break the one-to-one mapping between the message and coded message. Even with full understanding of the functioning of an encryption algorithm, the encrypted message cannot be recovered without a private key, which allows reversing the pseudo-randomness.

#### [Hypertrophy](Hypertrophy.pdf)

Muscle growth or hypertrophy occurs, when you send a signal to the body through resistance training, declaring that the current muscles are inadequate. As a response, protein is used to recover and improve the contracting filament -structure in the damaged muscle cells during the following days of rest. This document gives an overview of both the practicalities and the interesting cellular biology involved in the process.

### Profile

#### [CV](CV_Snellman.pdf)


### Simulations and Other Tools

#### [Simulate time series processes](Simulate%20time%20series%20-processes)

This simulator enables comparison of different time series processes, i.e. how identical shocks propagate differently in AR(1), MA(1), ARMA(1,1), GARCH(1,1) and ARMA-GARCH(1,1,1,1) models. If option IRF is specified as TRUE, then there is only one unit sized shock every 50 periods, otherwise the shocks are drawn randomly at each period from the specified distribution; normal, uniform or t-distribution (with df=10).  Coded in base R.

#### [Game of Life](Game%20of%20Life)

This R-code simulates the cellular automata, coined as The Game of Life by the mathematician John Conway. The Game of Life follows an iterative deterministic process based on simple rules, creating incredible and beautiful complexity. The starting configuration can be randomized or set by the user, alongside of the size of the arena.

#### [Monty Hall problem simulator](Monty%20Hall%20problem%20simulator)

In a famous probability puzzle you partake in Monty Hall game-show, where there are three doors from which you have to guess the correct one. After your initial guess the host (who knows which door holds the price) opens one of the remaining wrong ones, asking then "Would you like to change your pick to the remaining closed door?" Here is what makes this a puzzle: Sticking to your initial guess yields the prize 33% of the time, but changing the choice wins 66% of the time! The reason is that 66% of the time you choose wrong initially, leaving only the correct door left after the host's actions. But you don't need to take my word for it! Use my R-code to simulate as many Monty Hall games as you wish, and observe how many of them each strategy ends up winning. David Deutsch also had a brilliant comment on the matter: Monty Hall is not a Bayesian updating problem, but instead a (trivial) choice problem between two strategies (https://www.daviddeutsch.org.uk/2013/10/monty-hall-problem/).

#### [Frog jump simulator](Frog%20jump%20simulator)

This is a good example of the power of numeric (in contrast to analytic) approach to problem solving. Stand-up Maths (youtube-channel) explains an interesting probability puzzle: Frog crosses a river with 10 consecutive stones by jumping from a stone to another. The frog chooses randomly, to which of the remaining stones it jumps to. So at minimum, the crossing can be completed in one hop. At maximum, the frog visits each stone in order. What is the average number of jumps to cross this river? How does the average relate to the number of stones in the river? This is a hard problem to solve with a pen and paper, but it only took me 20 minutes to code a simulator, in which a frog crosses the river 100 000 times, resulting in an average of 2,9 jumps. This is a powerful shortcut to the answer, and can help you develop intuition about the problem. Can you figure out the relation between the average number of jumps and the total number of stones by using my R-simulator?

#### [Expected distance between points](Expected%20distance%20between%20points)

Have you always wondered, what is the expected distance between two random points in a unit square? What about the distance between two vectors in a (hyper)cube, with each side equal to one? Wait no more! With my R-code you can approximate the answer for any dimensions arbitrarily accurately! Fun thing to notice is that as the dimensions increase, the average distance between the points also increases monotonically without an upper limit, despite each side of the box having unit length.

#### [How to write your Thesis with LaTeX](How%20to%20write%20your%20Thesis%20with%20LaTeX%20-tutorial)

The aim of this document is to provide you with a LaTeX-template, with most of the common features and instructions on how to use them, so that you can successfully write your Master's thesis with LaTeX. To use my template, copy-paste the content into an empty Overleaf script. LaTeX is a document preparation system and a competitor of Word. It is very popular among quantitative scientists, because it makes writing equations enjoyable and aesthetic, among its many other benefits. Most of the pdf-documents on this page were produced with LaTeX.

