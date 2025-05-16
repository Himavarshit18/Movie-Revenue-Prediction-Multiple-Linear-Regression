# 🎬 Movie Revenue Prediction using Linear Regression (from Scratch)

This project implements multiple linear regression from scratch using NumPy to predict a movie's gross revenue. It includes feature scaling (z-score normalization), vectorized gradient descent, and learning rate tuning, all inside a Google Colab notebook.

---

## 📁 Dataset

The dataset includes the following features:

- `Budget` – Estimated production budget
- `Runtime` – Movie duration in minutes
- `Rating` – Average user rating (e.g., IMDb)
- `Rating Count` – Number of ratings submitted
- `release date_DD` – Day of the month the movie was released
- `release month_MM` – Month of the year the movie was released

**Target variable:**

- `Gross` – Gross revenue of the movie

---

## 🧪 Project Workflow

### Data Loading & Cleaning
- Read CSV file into Pandas DataFrame
- Drop rows with missing values

### Data Visualization
- Plot scatterplots of each feature vs. gross revenue

### Z-Score Normalization
- Standardize each feature using:
   x_norm = (x - μ) / σ
- Normalize target `Gross` for stable training

### Model Implementation
- Initialize weights `w` and bias `b`
- Vectorized computation of:
- Predictions
- Loss (MSE)
- Gradients
- Update parameters using Gradient Descent

### Learning Rate Tuning
- Try multiple learning rates (0.001 → 1.0)
- Plot learning curves to select the best fit

### Reverse Normalization
- Convert predicted values back to original scale:
  y = y_norm × σ + μ


### Evaluation
- Plot:
- Learning curves (Loss vs Epochs)
- Actual vs Predicted (normalized)
- Actual vs Predicted (original scale)
- Calculate:
- R² Score
- MSE (optional)

---

## 📊 Results

- Final R² Score: ~0.53  
- Gradient descent successfully converged after 500 epochs  
- Predictions align reasonably well with actual values  
- All model logic implemented manually using NumPy (no Scikit-learn)

---

## 📁 Files

- `movie_revenue_regression.ipynb` – Main Colab notebook  
- `README.md` – Project overview and structure  
- *(Optional)* `Movies_gross_rating.csv` – Input dataset

---

## 📌 How to Run

This project was built in **Google Colab**.

1. Upload the notebook and dataset to Colab  
2. Run all cells in order  
3. Tune learning rate and observe the impact  
4. Analyze the final prediction plots and metrics

---

## 🧑‍💻 Author

** Konuganti Himavarshit Reddy **
** Email: himavarshitreddyk@gmail.com **  
