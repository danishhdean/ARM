# Association Rule Mining with Apriori and FP-Growth
# 📝 Overview
This project implements Association Rule Mining using both the Apriori and FP-Growth algorithms in Python. It processes transaction data from an Excel dataset to identify frequent itemsets and generate association rules, visualized through scatter plots and network graphs for both algorithms.

# ✨ Features
Dual Algorithms: Implements Apriori and FP-Growth using mlxtend for mining frequent itemsets.

Rule Generation: Extracts association rules with metrics like support, confidence, and lift for both algorithms.

Visualizations: Generates scatter plots (support vs. confidence, colored by lift) and network graphs for rule relationships, for both Apriori and FP-Growth.

Data Preprocessing: Converts binary transaction data into item names using pandas and TransactionEncoder.

# 💬 How to Use
Load the dataset.

Run the script to preprocess transactions, apply both Apriori and FP-Growth, and generate rules.

View frequent itemsets and rules with metrics for each algorithm.

Explore visualizations (scatter plots and network graphs) for insights into item associations.

# 🧩 Project Structure
How It Works

Preprocessing: Loads Excel data, replaces binary values with item names, and prepares transactions using TransactionEncoder.

Apriori Algorithm: Uses mlxtend.apriori to find frequent itemsets with a minimum support threshold (0.3) and generates rules with a confidence threshold (0.6).

FP-Growth Algorithm: Uses mlxtend.fpgrowth to find frequent itemsets with the same support threshold and generates rules with the same confidence threshold.

Visualization:

Scatter plots (support vs. confidence) for both algorithms, with lift as the color scale.

Network graphs using networkx to show rule relationships for both algorithms.

# ⚠️ Limitations
Requires a well-structured binary dataset.

Performance depends on chosen support and confidence thresholds.

Apriori may be slower than FP-Growth for large datasets.

Visualizations may become cluttered with many rules.

No handling for missing or inconsistent data.

# 🚀 Future Improvements
Incorporate dynamic threshold tuning for better rule quality.

Add performance benchmarking to compare Apriori and FP-Growth runtimes.

Enhance visualizations with interactive elements.

Support larger datasets with parallel processing.
