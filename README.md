# CATALOG_ASSIGNMENT

# Simplified Shamir's Secret Sharing Assignment

## Overview

In this assignment, you'll implement a simplified version of Shamir's Secret Sharing algorithm to find the constant term of a polynomial. Given a polynomial of degree \( m \), you need to find the constant term \( c \) using \( m+1 \) roots of the polynomial. The polynomial is represented as:

\[ f(x) = a_m x^m + a_{m-1} x^{m-1} + \dots + a_1 x + c \]

Where:
- \( f(x) \) is the polynomial function.
- \( m \) is the degree of the polynomial.
- \( a_m, a_{m-1}, \dots, a_1, c \) are the coefficients of the polynomial, with \( a_m \neq 0 \).

## Objective

Given the roots of the polynomial in a specific format, you need to compute the constant term \( c \). The roots are provided in a JSON format which will be parsed and used to determine the polynomial's constant term.

## Features

- **JSON Input Handling**: Read and parse JSON input that provides the necessary data for polynomial evaluation.
- **Polynomial Computation**: Use Lagrange interpolation to determine the polynomial's constant term from the given roots.
- **Error Handling**: Handle cases where the input format is incorrect or insufficient data is provided.

## Technologies Used

- **JavaScript**: For implementing the logic to parse input, perform Lagrange interpolation, and compute the constant term.
- **HTML/CSS**: To create a simple user interface for uploading and processing the JSON file.

## File Structure

- `index.html`: Contains the HTML structure for the user interface.
- `styles.css`: Provides styling for the HTML elements.
- `script.js`: Contains JavaScript code for handling file input, parsing JSON, computing the polynomial's constant term, and displaying the result.





Copy this code in index.html file and run the code.

You will see a choose a file button. After clicking on the button choose a file with .json extension with any name where the test case is input:

The input format of .json file test case is :

Test Case 1 :

{ "keys": { "n": 4, "k": 3 }, "1": { "base": "10", "value": "4" }, "2": { "base": "2", "value": "111" }, "3": { "base": "10", "value": "12" }, "6": { "base": "4", "value": "213" } }

Test Case 2 :

{ "keys": { "n": 9, "k": 6 }, "1": { "base": "10", "value": "28735619723837" }, "2": { "base": "16", "value": "1A228867F0CA" }, "3": { "base": "12", "value": "32811A4AA0B7B" }, "4": { "base": "11", "value": "917978721331A" }, "5": { "base": "16", "value": "1A22886782E1" }, "6": { "base": "10", "value": "28735619654702" }, "7": { "base": "14", "value": "71AB5070CC4B" }, "8": { "base": "9", "value": "122662581541670" }, "9": { "base": "8", "value": "642121030037605" } }


index file has been updated

