## 🌳 Why Decision Tree Model?

We used **DecisionTreeClassifier** because:

* ✅ Easy to understand and visualize
* ✅ Works well with both numerical and categorical data
* ✅ No need for heavy preprocessing (like normalization, though we used it for pipeline consistency)
* ✅ Handles non-linear relationships
* ✅ Fast training and prediction

👉 In this dataset, survival depends on conditions like:

* Gender (female had higher survival)
* Passenger class
* Age
  A Decision Tree can easily split data based on these rules.

---

## ⚙️ How Decision Tree Works

A Decision Tree works like a **flowchart**:

1. It splits the dataset based on a feature
2. Chooses the best split using a metric (like Gini or Entropy)
3. Repeats splitting until:

   * Data becomes pure, or
   * Maximum depth is reached

---

## 🌿 Example of Decision Flow

```
Is Sex = Female?
        /       \
     Yes         No
    /             \
Survived?     Is Age < 10?
                 /     \
              Yes       No
           Survived   Not Survived
```

---

## 📊 How Model Makes Decisions

* The model checks features step by step
* At each step, it asks a question (condition)
* Based on the answer, it moves left or right
* Finally, it reaches a **leaf node** (prediction)

---

## 🧠 Important Concepts

### 1. Gini Impurity

* Measures how mixed the classes are
* Lower value = better split

### 2. Entropy

* Measures randomness in data
* Used to calculate Information Gain

### 3. Information Gain

* Helps choose the best feature to split

---

## ⚠️ Limitations of Decision Tree

* ❌ Can overfit easily
* ❌ Sensitive to small data changes
* ❌ Not as powerful as ensemble models

---

## 💡 Why It Works Well for Titanic Dataset

* Dataset is small and structured
* Clear decision rules exist
* Relationships are not too complex

👉 That’s why Decision Tree gives good accuracy (~77%)

---

## 🚀 Better Alternatives (Optional)

For improvement, you can try:

* Random Forest (reduces overfitting)
* Gradient Boosting
* XGBoost

---
