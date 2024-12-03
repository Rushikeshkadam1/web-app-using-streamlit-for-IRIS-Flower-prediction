# Iris Species Classification with Random Forest

## Aim

The aim of this project is to develop an interactive machine learning application that predicts the species of an Iris flower based on its physical characteristics using a Random Forest Classifier. The application leverages the Iris dataset, a commonly used dataset in machine learning, and provides users with an easy-to-use interface for predicting the species based on four input features: sepal length, sepal width, petal length, and petal width.

## Methodology

The methodology behind this project involves the following key components:

1. **Dataset**: The dataset used is the Iris dataset, which contains measurements of 150 Iris flowers from three different species. The dataset includes four features: sepal length, sepal width, petal length, and petal width, along with the corresponding species label.
   
2. **Model**: A Random Forest Classifier is used to train a predictive model on the Iris dataset. This model is capable of classifying the species of an Iris flower based on the input features.

3. **Streamlit Interface**: A Streamlit application is developed to create an interactive user interface. Users can input values for the four features, and the model will predict the corresponding species.

4. **Prediction**: When the user provides values for the sepal and petal measurements via sliders in the sidebar, the application generates a prediction using the trained Random Forest model. The predicted species is displayed on the main interface.

5. **Caching**: To improve performance, the dataset loading and model training process is cached using Streamlit’s `@st.cache` decorator.

## Evaluation Metric

The model's performance is evaluated based on the accuracy of the predictions made by the Random Forest Classifier. In this case, the Iris dataset is well-known and typically achieves high classification accuracy with Random Forest due to the simple and separable nature of the data.

- **Accuracy**: This is the proportion of correct predictions made by the model compared to the total number of predictions.
- **Confusion Matrix**: While not visualized in the application, a confusion matrix can be used to assess how well the model distinguishes between the three Iris species.

## Results

The Random Forest model is trained on the Iris dataset, and when a user inputs the four flower measurements (sepal length, sepal width, petal length, and petal width), the model predicts the species of the flower. 

For example:

**Input:**
- Sepal Length: 5.1 cm
- Sepal Width: 3.5 cm
- Petal Length: 1.4 cm
- Petal Width: 0.2 cm

**Prediction:**
The predicted species is **Setosa**.

The application uses sliders to input the values and returns the species prediction after evaluating the model.

## Conclusion

This project demonstrates the practical use of machine learning to classify Iris flower species based on physical characteristics. The Random Forest Classifier provides an accurate and reliable model for prediction. The integration with Streamlit allows users to interact with the model easily, making the prediction process accessible to anyone without requiring any coding knowledge. This application serves as a great example of building interactive ML applications with user-friendly interfaces.

## Future Work

1. **Model Improvements**: Experiment with other machine learning models like Support Vector Machines (SVM), k-Nearest Neighbors (k-NN), or Gradient Boosting to see if they outperform the Random Forest Classifier on this dataset.
   
2. **Advanced Visualization**: Implement additional visualizations such as feature importance plots, pair plots, or decision boundary plots to help users better understand how the model works and the relationships between features.
   
3. **Expand Dataset**: Use larger or more complex datasets for flower species classification to test the scalability and adaptability of the model.
   
4. **Cross-Validation**: Implement cross-validation techniques to assess the model's performance more rigorously and reduce overfitting.

5. **Web Deployment**: Deploy the Streamlit app on a web server so that users can access it remotely from anywhere, improving accessibility and user experience.

## How to Run

### Prerequisites
- Python 3.x
- Required Python packages from `requirements.txt`

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/username/Iris-Species-Classification.git
   cd Iris-Species-Classification
   ```
2. Install the dependencies:
```bash
pip install -r requirements.txt
```
3. Run the Streamlit application:
```bash
streamlit run classification.py
```
4. Open the provided local URL in your browser to use the app.
