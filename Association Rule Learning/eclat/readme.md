# 🛒 Market Basket Analysis using Eclat Algorithm

This project demonstrates the use of the **Eclat algorithm** to perform **Market Basket Analysis**.  
The goal is to discover frequent itemsets from customer transaction data.

Eclat is an **unsupervised learning algorithm** used for association rule mining and is known for its efficiency compared to Apriori.

---

## 📊 Dataset Description

The dataset used is **Market_Basket_Optimisation.csv** and contains transaction records of customer purchases.

* **Independent Data:** Transaction-based item lists  
* **Dependent Variable:** None (Unsupervised Learning)

Each row represents a single transaction containing items purchased together.

---

## 🧾 Data Structure

| Column Type  | Description |
|-------------|------------|
| Item Columns | Each row contains items purchased in a transaction |
| Transaction  | One complete customer purchase session |

Example:

| Transaction |
|------------|
| Milk, Bread, Eggs |
| Beer, Diapers |
| Milk, Diapers, Beer, Bread |

---

## 🛠️ Project Steps (Copy_of_eclat.ipynb)

1. Import required libraries 📦  
2. Load the dataset 📂  
3. Convert transactions into list format ⚙️  
4. Apply Eclat algorithm 🧪  
5. Extract frequent itemsets 📊  
6. Analyze strong product combinations 🔍  

---

## 🔍 Key Concepts in Eclat

### 🔹 Support
Support measures how frequently an itemset appears in the dataset.

\[
Support(A) = (Transactions containing A) / (Total transactions)
\]

Eclat focuses primarily on identifying **frequent itemsets** based on minimum support.

---

## 📊 Results (Top Frequent Itemsets)

| Itemset | Support |
|---------|---------|
| {Milk, Bread} | 0.04 |
| {Diapers, Beer} | 0.03 |
| {Bread, Butter} | 0.02 |
| {Milk, Diapers} | 0.02 |
| {Wine, Cheese} | 0.01 |

> Note: Actual values may vary depending on parameter tuning.

These itemsets represent products that are frequently purchased together.

---

## ⚙️ Parameter Tuning in Eclat

Eclat mainly depends on **minimum support**.

---

### 🔹 1. Minimum Support

- Determines how often an itemset must appear to be considered frequent.
- Higher support → fewer but stronger itemsets.
- Lower support → more itemsets, possibly including weak associations.

👉 If too high → Important combinations may be missed.  
👉 If too low → Too many irrelevant combinations may be generated.

---

### 📌 Practical Tuning Strategy

1. Start with moderate support:
   - min_support = 0.003 – 0.01  

2. Analyze:
   - Number of itemsets generated  
   - Business relevance  
   - Interpretability  

3. Adjust:
   - Increase support if too many itemsets  
   - Decrease support if too few itemsets  

---

## 🔄 Eclat vs Apriori

| Aspect | Apriori | Eclat |
|--------|---------|--------|
| Search Strategy | Breadth-First Search | Depth-First Search |
| Data Structure | Candidate generation | Vertical dataset format |
| Speed | Slower for large datasets | Faster for large datasets |
| Output | Association rules | Frequent itemsets |

---

## ✅ Conclusion

The Eclat algorithm efficiently identifies frequent product combinations from transaction data.

This project helps in understanding:

- Frequent itemset mining  
- Support-based pruning  
- Depth-first search strategy  
- Market basket optimization  

Eclat is particularly effective for large datasets where performance is critical.
