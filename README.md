# Student Exam Score Prediction (TensorFlow)

A mini machine learning project exploring how student study habits and lifestyle factors
affect exam performance.  
Built and trained a **supervised neural network (TensorFlow)** to predict exam scores.

---

##  Project Overview
- **Goal:** Predict students’ final exam scores using study and lifestyle data.
- **Dataset:** [Student Habits vs Academic Performance (Kaggle)](https://www.kaggle.com/datasets/jayaantanaath/student-habits-vs-academic-performance)
- **Type:** Supervised regression using neural networks

---

##  Features
| Feature | Description |
|----------|--------------|
| `age` | Student’s age |
| `study_hours_per_day` | Average daily study hours |
| `social_media_hours` | Average social media use per day |
| `attendance_percentage` | Attendance in class (%) |
| `sleep_hours` | Average sleep per night |
| `mental_health_rating` | Self-rated mental health (1–10) |
| **Target:** `exam_score` | Final exam score |

---

##  Model Details
- **Algorithm:** Feed-forward Neural Network (Keras / TensorFlow)
- **Architecture:** 2 hidden layers (64 → 32 neurons, ReLU)
- **Regularization:** Dropout (0.2) + L2
- **Optimizer:** Adam (learning rate = 0.001)
- **Loss:** MSE
- **Metrics:** MAE, RMSE, R²

---

## 📊 Results
| Metric | Score |
|---------|--------|
| MAE | **5.61** |
| RMSE | **7.05** |
| R² | **0.82** |

> The model explains ~82% of the variance in student performance — a strong fit for this dataset.

---

##  Visualization
![pred-vs-actual](your_plot_image.png)
*(Scatter plot showing predicted vs actual exam scores — points align closely with the ideal line.)*

---

## 💡 Key Insights
- Higher study hours and attendance correlate strongly with higher exam scores.
- Excessive social media time and low sleep negatively affect performance.
- Balanced lifestyle factors (study + rest) lead to better results.

---

##  Tools Used
- Python, Jupyter Notebook  
- TensorFlow / Keras  
- Scikit-learn  
- Matplotlib, Pandas, NumPy  

---

## How to Run
```bash
git clone https://github.com/<pharoh673>/student-performance-ml.git
cd student-performance-ml
pip install -r requirements.txt
jupyter notebook
