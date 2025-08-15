# Random-Forest-From-Scratch
Machine learning Algorithms From Scratch

---

## ⚙️ Implementation Steps

1. **Data Preprocessing**
   - Handle missing values (median for numeric, mode for categorical)
   - Encode categorical variables into numeric form
   - Normalize/standardize features if necessary
   - Split dataset into training and testing sets

2. **Decision Tree from Scratch**
   - Implement splitting criterion using **Gini Impurity**
   - Build tree recursively
   - Set a maximum depth and minimum samples per split to avoid overfitting

3. **Bootstrap Sampling**
   - Randomly sample data with replacement to train each tree

4. **Random Feature Selection**
   - At each node, choose a random subset of features to consider for splitting

5. **Random Forest Construction**
   - Train multiple decision trees on different bootstrap samples
   - Store all trained trees

6. **Prediction**
   - Each tree predicts independently
   - Final prediction is based on **majority voting**

7. **Evaluation**
   - Measure accuracy on test data
   

---

## 🧠 Key Concepts

- **Bagging (Bootstrap Aggregating)**: Training multiple models on random subsets of the data
- **Feature Randomness**: Choosing random features at each split to increase diversity among trees
- **Entropy**: Metric to measure node randomness in classification
- **Majority Voting**: Combining predictions from all trees

---

## 📊 Results

- **Random Forest Accuracy**: ~81% (depends on hyperparameters & preprocessing)
- Outperforms single Decision Tree in terms of stability and generalization

---

## 🛠 Requirements

Install the required libraries before running:

```bash
numpy,pandas
