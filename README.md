# Song-Genre-Guesser-ML-Model

This project is a machine learning model that predicts music genres based on age and gender. It uses a decision tree classifier to analyze the relationship between a person's age, gender, and their preferred music genre.

## Features

- **Model Training**: The model is trained on a dataset containing age, gender, and music genre information.
- **Prediction**: Users can input their age and gender to receive predictions on their preferred music genre.
- **Model Persistence**: The trained model is saved using the `joblib` library for future use.

## Dataset

The project uses a dataset called `music.csv`, which includes the following columns:

- **age**: The age of the person.
- **gender**: The gender of the person (encoded as 1 for male and 0 for female).
- **genre**: The music genre preferred by the person.

## Project Structure

- **`Project 1 py.ipynb`**: Jupyter notebook containing the code for data processing, model training, prediction, and saving the trained model.
- **`music.csv`**: The dataset used for training the model.
- **`music-recommender.dot`**: Visualization of the decision tree generated by the model.
- **`music-recommender.joblib`**: The saved model for future predictions.

## Usage

### Training the Model

The model is trained using a decision tree classifier. The training process involves:

1. Loading the dataset using `pandas`.
2. Splitting the data into features (`age` and `gender`) and the target variable (`genre`).
3. Training the decision tree model on the data.
4. Exporting the decision tree structure to a `.dot` file for visualization.

### Making Predictions

After training the model, you can make predictions by providing a 2D array containing age and gender values.

```python
predictions = model.predict([[age, gender]])
print(predictions)


