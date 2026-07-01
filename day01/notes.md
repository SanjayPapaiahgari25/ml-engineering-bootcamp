# Day 1 - Introduction to Machine Learning

## Lecture
Mathematical Foundations of Machine Learning

---

# Objective

Understand what Machine Learning is and how a learning problem is formulated mathematically.

---

# What is Machine Learning?

Machine Learning is the process of learning an unknown function from data.

Instead of writing explicit rules, we provide examples (training data), and the algorithm estimates a function that maps inputs to outputs.

Mathematically,

f : X → Y

where

- X = Input Space
- Y = Output Space
- f = Unknown function to be learned

---

# Learning Problem

Given a dataset

D = {(x₁, y₁), (x₂, y₂), ..., (xₙ, yₙ)}

learn an approximation of the unknown function f that can predict outputs for unseen inputs.

---

# Components of a Learning Problem

## Input Space (X)

Examples:

- House features
- X-ray image
- Customer information
- Email text

---

## Output Space (Y)

Examples:

- House price
- Disease / No Disease
- Spam / Not Spam
- Customer Churn

---

## Dataset

A dataset consists of input-output pairs.

(x₁, y₁)

(x₂, y₂)

...

(xₙ, yₙ)

---

# Function Approximation

The true function is unknown.

Machine Learning estimates a function

f̂

that approximates the true mapping.

Goal:

Estimated Function ≈ True Function

---

# Image Representation

If an image contains

- P pixels horizontally
- Q pixels vertically

then

Number of pixels = P × Q

Each pixel value becomes one feature.

The image is flattened into a one-dimensional vector before being given to classical Machine Learning algorithms.

Example

Image

1 2 3
4 5 6

↓

Vector

[1, 2, 3, 4, 5, 6]

---

# Important Note

The symbols P and Q are only notation.

In this lecture,

- P = Horizontal pixel count
- Q = Vertical pixel count

Therefore,

- Number of columns = P
- Number of rows = Q

Different books or papers may define them differently.

Always follow the author's definitions.

---

# Why Flatten an Image?

Classical Machine Learning algorithms expect a feature vector as input.

For an image,

Number of Features = Number of Pixels

d = P × Q

Input vector

x ∈ ℝᵈ

---

# Statistical Learning

Machine Learning estimates the best function from observed data instead of memorizing rules.

The objective is to generalize well to unseen data.

---

# Key Takeaways

- Machine Learning learns an unknown function from data.
- A dataset is a collection of input-output pairs.
- The learning objective is to estimate f : X → Y.
- Images are converted into vectors for classical Machine Learning.
- Number of image features = Number of pixels.
- Always understand the notation used by the author instead of assuming symbol meanings.

---

# Interview Notes

Q. What is Machine Learning?

Machine Learning is the process of estimating an unknown mapping function from input space to output space using training data, so that it can generalize to unseen examples.

---

# My Understanding

- Machine Learning is fundamentally a function approximation problem.
- Data is more important than manually writing rules.
- Images must be represented numerically before they can be processed by ML algorithms.
- Mathematical notation depends on the author's definitions and should not be assumed.
- I should focus on understanding concepts rather than memorizing formulas.

---

# Questions I Had

- Why are images converted into vectors?
- Why were P and Q used for horizontal and vertical dimensions?
- Why does NumPy use (rows, columns) while the lecture used different notation?

Resolved:
Yes. NumPy follows the (rows, columns) convention, while the professor defined P and Q based on horizontal and vertical pixel counts. Both are correct as long as the notation is used consistently.

---

# Practical Exercise

- Created a 3×4 image using NumPy.
- Printed the image.
- Flattened it into a vector.
- Verified that:

Number of Pixels = Number of Features

This demonstrates why classical Machine Learning models operate on vectors rather than image matrices.
