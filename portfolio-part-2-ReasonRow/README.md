# portfolio-part-2-ReasonRow

# Machine Learning Model Training & Testing

This project demonstrates how to create training and testing sets, apply a linear regression model, and evaluate performance using error metrics.  

---

## 📌 Project Objective
The goal of this project was to establish a **training and testing model** — a fundamental step in machine learning that helps evaluate accuracy and performance.

- **Case 1:** 10% training data, 90% testing data  
- **Case 2:** 90% training data, 10% testing data  

These splits allowed us to compare model performance under different training/testing scenarios.

---

## 🔍 Exploration
We used a **linear regression model** to explore how various features correlate with the target variable (**rating**).  

Key steps:
1. **Feature Exploration:** Identified features such as `helpfulness`, `gender`, `category`, and `review` and assessed their relationship with ratings.  
2. **Dataset Splitting:** Created training and testing sets using the percentages above.  
3. **Model Training:** Applied regression models in several scenarios (Cases A–D), using either the two most correlated or two least correlated features.  
4. **Model Evaluation:** Measured performance using **Mean Squared Error (MSE)** and **Root Mean Squared Error (RMSE)** and plotted results for visual comparison.  

---

## 🧩 Additional Features
- Clear **comments** throughout the code to explain:
  - The purpose of each step  
  - The type of data being processed  
  - Expected outputs  

---

## 🚧 Challenges
Some of the main challenges included:  
- Understanding the task requirements and clarifying objectives  
- Learning and applying **Ordinal Encoder** correctly  
- Training and testing multiple models to ensure accuracy  
- Finding and using the correct formula for **MSE**, given several available options  

---

## 💡 Future Improvements
Planned enhancements for this project include:  
- Improving the graph’s appearance for better clarity  
- Refactoring the code for improved readability
- Refining comments to make the logic even easier to follow  
