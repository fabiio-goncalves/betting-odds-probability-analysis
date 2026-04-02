# Betting Odds Probability Analysis

This project explores how betting odds can be translated into probabilities and used to evaluate bets using basic statistical and data science techniques.

The objective is to demonstrate how simple models can be applied to estimate match outcomes and support decision-making in a betting context.

---

## Overview

In sports betting, odds represent implied probabilities of events. However, these probabilities can be analysed, adjusted, and compared with model-based estimates.

This project implements a small analytical pipeline that:

- Converts betting odds into probabilities  
- Calculates expected value (EV)  
- Models win probability using a logistic function  
- Estimates score distributions using a Poisson model  
- Simulates match outcomes using Monte Carlo methods  

---

## Methodology

### 1. Odds to Probability

Decimal odds are converted into implied probabilities:

Probability = 1 / Odds

---

### 2. Expected Value

Expected Value (EV) is used to evaluate if a bet is favourable:

EV = (Probability × Odds) - 1

---

### 3. Logistic Model

A logistic function is used to model the probability of winning based on goal difference.

---

### 4. Poisson Distribution

The Poisson distribution is used to model the number of goals scored by each team and generate a score probability matrix.

---

### 5. Monte Carlo Simulation

Match outcomes are simulated multiple times to approximate:

- Home win probability  
- Draw probability  
- Away win probability  

---

## Results

### Win Probability Model

![Win Probability](logistic_curve.png)

This curve shows how the probability of winning varies with goal difference.

---

### Score Distribution

![Score Matrix](poisson_matrix.png)

This matrix represents the probability of each possible score using the Poisson model.

---

## Key Insights

- Betting odds can be interpreted as probabilities  
- Expected Value helps identify profitable bets  
- The Poisson distribution is effective for modelling football scores  
- Simulated results align with analytical estimates  

---

## Technologies

- Python  
- NumPy  
- Pandas  
- Matplotlib  

---

## How to Run

Install dependencies:

```bash
pip install numpy pandas matplotlib
```
Run the script:

```bash
python analysis.py
```
