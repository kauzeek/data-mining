# data-mining
# Data Mining Project

This project implements the Apriori and FP Growth (FP Tree) algorithms to find the maximal frequent itemsets from a given dataset (`store_data.csv`).

## Algorithms Implemented

### 1. Apriori Algorithm
The Apriori algorithm is implemented from scratch and also using the `mlxtend` library for comparison.

#### Apriori Algorithm Without Built-In Functions
- **Steps:**
  - Load and preprocess the dataset.
  - Generate candidate itemsets.
  - Calculate support counts and filter itemsets based on minimum support.
  - Repeat until no more itemsets can be generated.

#### Apriori Algorithm Using Built-In Functions
- Utilizes the `mlxtend` library to quickly generate frequent itemsets.
- This implementation is used to verify the results from the custom implementation.

### 2. FP Growth Algorithm
The FP Growth algorithm is implemented from scratch to find frequent itemsets.

#### FP Growth Algorithm Without Built-In Functions
- **Steps:**
  - Construct an FP Tree from the dataset.
  - Extract frequent itemsets by mining the FP Tree.
  - Build conditional trees and recursively mine them to generate itemsets.

## Getting Started

### Prerequisites
- Python 3.x
- Pandas library
- `mlxtend` library (for the Apriori implementation using built-in functions)

### Installation
To install the required libraries, run:
```bash
pip install pandas mlxtend
