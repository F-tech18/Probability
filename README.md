# Module 13 – Probability

## Project Overview
This assignment explores probability through Python simulations, conditional probability, Bayes' theorem, random variables, continuous distributions, and the Central Limit Theorem. The notebook includes code, Markdown explanations, and visualizations.

## Objectives
- Estimate probabilities through repeated random experiments.
- Simulate coin tosses and dice rolls.
- Estimate conditional probabilities and check Bayes' theorem.
- Generate samples from a discrete random variable and calculate descriptive statistics.
- Visualize an exponential distribution with a theoretical probability density function (PDF).
- Demonstrate the Central Limit Theorem using sample means.

## Tools and Libraries
- Python
- Jupyter Notebook
- `random` (standard Python library)
- NumPy
- Matplotlib

## Project Structure
```text
Module_13_Probability_Assignment/
├── Module_13_Probability_Assignment.ipynb
└── README.md
```

## Assignment Tasks

### 1. Basics of Probability
- Simulate 10,000 coin tosses and calculate experimental probabilities for heads and tails.
- Simulate rolling two dice and estimate the probability that their sum is 7.
- Use loops to run repeated trials and count outcomes.

### 2. At Least One Six
- Simulate 10 rolls of a fair die per trial.
- Repeat the experiment many times.
- Estimate the proportion of trials containing at least one six.
- Compare the simulation with the theoretical probability: `1 - (5/6)**10`.

### 3. Conditional Probability and Bayes' Theorem
A bag contains 5 red, 7 green, and 8 blue balls. Each ball is replaced after being drawn.
- Simulate consecutive draws and estimate the probability that a draw is red given that the previous draw was blue.
- Estimate the joint and marginal probabilities from the simulation.
- Verify Bayes' theorem using the events `A = current draw is red` and `B = previous draw is blue`:
  `P(A|B) = P(B|A) * P(A) / P(B)`.
- Since draws are independent with replacement, the expected value of `P(A|B)` is `5/20 = 0.25`.

### 4. Discrete Random Variable
Generate 1,000 observations with:
- `P(X=1) = 0.25`
- `P(X=2) = 0.35`
- `P(X=3) = 0.40`

Calculate the empirical mean, variance, and standard deviation using NumPy.

### 5. Continuous Random Variable
- Generate 2,000 observations from an exponential distribution with mean 5 (scale parameter 5).
- Plot a density-normalized histogram.
- Overlay the theoretical exponential PDF: `f(x) = (1/5) * exp(-x/5)` for `x >= 0`.

### 6. Central Limit Theorem
- Generate a population of 10,000 values from a uniform distribution.
- Draw 1,000 samples of size 30 with replacement from this population.
- Calculate the mean of each sample.
- Compare the uniform population distribution with the distribution of sample means.

## Installation and Setup

Install the required libraries:
```bash
python -m pip install numpy matplotlib notebook
```

Launch Jupyter Notebook from the assignment folder:
```bash
python -m notebook
```

Open `Module_13_Probability_Assignment.ipynb` and run the cells from top to bottom. All plots and printed outputs should be visible before submission.

## Expected Results
- Experimental probabilities for coin tosses and dice rolls.
- An estimated probability for at least one six in ten die rolls, with a theoretical comparison.
- Simulation-based conditional probability and a Bayes' theorem verification.
- Empirical statistics for the discrete random variable.
- An exponential-distribution histogram with a theoretical PDF overlay.
- A comparison between a uniform population and the sampling distribution of sample means.

## Submission Checklist
- [ ] Run every code cell without errors.
- [ ] Keep the Markdown explanations for each section.
- [ ] Ensure all printed outputs and plots are visible.
- [ ] Save the completed notebook in `.ipynb` format.
- [ ] Include this `README.md` when submitting the project.

## Conclusion
This assignment provides practical experience using simulation to understand probability and statistical concepts. It connects theoretical probability with empirical estimates and visualizes important ideas such as distributions and the Central Limit Theorem.
