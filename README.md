# pc_price_guessing

# Computer Price Prediction Project

This project aims to predict the price of a computer based on its technical specifications (RAM, CPU, GPU, etc.). It uses a dataset from Kaggle.

## Project Goal: Comparing Two Methods

The main goal of this project was to try two different machine learning methods on the same problem and see which one performs better:

1.  **Baseline Model:** First, we established a baseline prediction using a simple and fast model: **Linear Regression** (with the Scikit-learn library).
2.  **Advanced Model:** Then, we built a **Deep Neural Network** (with the TensorFlow/Keras library), which can learn more complex relationships.

Our goal was to answer the question: "On this problem, how much better is a complex deep learning model compared to a simple linear regression model?"

## 🚀 Tools Used

* Python
* Pandas (For reading and cleaning data)
* Scikit-learn (For Linear Regression and data scaling)
* TensorFlow / Keras (For the Deep Neural Network model)
* Matplotlib (For visualizing results)
* KaggleHub (To automatically download the dataset)

## 🏁 How to Run

1.  **Install the required libraries:**
    `(A 'requirements.txt' file is included in the project folder)`
    ```bash
    pip install -r requirements.txt
    ```

2.  **Run the script:**
    When executed, the script will automatically download the dataset, train the models, and save the result graphs (as `.png` files) into the same folder.
    ```bash
    python pc_price_guess.py
    ```

## 📊 Results and Conclusion

Results obtained on the test data:

| Model | R-squared (R2) | Mean Absolute Error (MAE) |
| :--- | :--- | :--- |
| Linear Regression | ~0.8747 | ~143.77 TL |
| Neural Network (DNN) | ~0.8783 | ~141.10 TL |

### Conclusion

Looking at the results, we see that both models were quite successful, with an R2 score of (~87%). The Neural Network model performed slightly better than the Linear Regression model (reducing the error by ~2.6 TL).

This shows that for this specific dataset, a simple Linear Regression model can be almost as successful as a deep learning model.
