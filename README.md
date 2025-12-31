# Floating-Point Error Lab

This repository explores **floating-point error**, **numerical stability**, and **conditioning** through a series of numerical experiments. The goal is to better understand *why* floating-point computations break down in certain cases, *how* these failures appear in practice, and *how* rewriting formulas in a numerically stable way can significantly improve accuracy without increasing precision.

Rather than treating floating-point arithmetic as a black box, this project investigates its behavior using concrete examples, standard error metrics, and high-precision reference values to make sources of numerical error explicit.

## Notebook Overview

### `00_setup_and_metrics.ipynb`
Establishes the experimental foundation:
* IEEE-754 floating-point overview
* Absolute and relative error metrics
* High-precision reference values using arbitrary-precision arithmetic
* A worked example demonstrating catastrophic cancellation in $1-\cos(x)$

### `01_machine_epsilon.ipynb`
Explores floating-point precision limits:
* Definition and computation of machine epsilon
* Experimental verification for **float32** and **float64**
* Interpretation of precision as relative spacing near $1.0$
* Connection between machine epsilon and loss of significance