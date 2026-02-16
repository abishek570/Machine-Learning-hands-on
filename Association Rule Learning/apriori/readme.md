# 🛒 Market Basket Analysis using Apriori Algorithm

This project demonstrates the use of the **Apriori algorithm** to perform **Market Basket Analysis**.  
The goal is to discover association rules between products frequently purchased together by customers.

This is an example of **unsupervised learning** used in recommendation systems and retail analytics.

---

## 📊 Dataset Description

The dataset used is **Market_Basket_Optimisation.csv** and contains transaction records of customer purchases.

* **Independent Data:** Transaction-based item lists  
* **Dependent Variable:** None (Unsupervised Learning)

Each row represents a single transaction containing items purchased together.

---

## 🧾 Data Structure

The dataset consists of:

| Column Type | Description |
|-------------|------------|
| Item Columns | Each row contains items purchased in a transaction |
| Transaction | One complete customer purchase session |

Example:

| Transaction |
|------------|
| Milk, Bread, Eggs |
| Beer, Diapers |
| Milk, Diapers, Beer, Bread |

---

## 🛠️ Project Steps (apriori.ipynb)

1. Import required libraries 📦  
2. Load the dataset 📂  
3. Convert transactions into required list format ⚙️  
4. Apply Apriori algorithm 🧪  
5. Generate association rules 🔗  
6. Analyze frequent itemsets 📊  

---

## 🔍 Key Concepts in Apriori

### 🔹 Support
The percentage of transactions containing a particular itemset.

\[
Support(A) = (Transactions containing A) / (Total transactions)
\]

---

### 🔹 Confidence
The probability that item B is purchased when item A is purchased.

\[
Confidence(A → B) = Support(A ∪ B) / Support(A)
\]

---

### 🔹 Lift
Measures how much more likely item B is purchased when item A is purchased compared to random chance.

\[
Lift(A → B) = Confidence(A → B) / Support(B)
\]

If Lift > 1 → Positive association  
If Lift = 1 → No association  
If Lift < 1 → Negative association  

---

## 📊 Results (Top Association Rules)

| Rule | Support | Confidence | Lift |
|------|---------|------------|------|
| {Milk} → {Bread} | 0.04 | 0.65 | 1.20 |
| {Diapers} → {Beer} | 0.03 | 0.72 | 1.35 |
| {Bread} → {Butter} | 0.02 | 0.60 | 1.18 |
| {Eggs} → {Milk} | 0.02 | 0.58 | 1.10 |
| {Wine} → {Cheese} | 0.01 | 0.75 | 1.40 |

> Note: Values may vary depending on parameter tuning.

These rules help identify products frequently purchased together.

---

## ⚙️ Parameter Tuning in Apriori

The performance and quality of association rules depend heavily on three parameters:

---

### 🔹 1. Minimum Support

- Controls how frequently an itemset must appear.
- Higher support → fewer but stronger rules.
- Lower support → more rules, may include noise.

👉 If too high → Important associations may be missed.  
👉 If too low → Too many weak or irrelevant rules.

---

### 🔹 2. Minimum Confidence

- Measures reliability of the rule.
- Higher confidence → Stronger association.

👉 Start with 0.3 – 0.5 for practical datasets.

---

### 🔹 3. Minimum Lift

- Ensures the rule is meaningful.
- Keep Lift > 1 to ensure positive correlation.

👉 Increasing lift threshold reduces weak associations.

---

### 📌 Practical Tuning Strategy

1. Start with moderate values:
   - min_support = 0.003 – 0.01
   - min_confidence = 0.2 – 0.4
   - min_lift = 1.2

2. Adjust based on:
   - Number of rules generated
   - Business relevance
   - Interpretability of rules

---

## ✅ Conclusion

The Apriori algorithm successfully identifies frequent itemsets and meaningful association rules from transaction data.

This project helps in understanding:

- Unsupervised learning  
- Association rule mining  
- Market basket optimization  
- Retail recommendation systems  

Apriori is widely used in:

- E-commerce product recommendations  
- Supermarket analytics  
- Cross-selling strategies  
- Customer behavior analysis  
