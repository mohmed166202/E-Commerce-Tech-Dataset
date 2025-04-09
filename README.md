# E-Commerce Tech Dataset Analysis

This project analyzes an e-commerce dataset and builds a machine learning model to predict product ratings. It also provides a recommendation system to suggest the top N products based on predicted ratings.

## Features
- **Data Cleaning**: Handles missing values, cleans price and rating columns, and normalizes numerical features.
- **Machine Learning Model**: Implements a neural network using TensorFlow to predict product ratings.
- **Recommendation System**: Recommends the top N products based on predicted ratings.
- **Visualization**: Visualizes the relationship between true and predicted ratings.

## Dataset
The dataset is stored in a CSV file located at:
`/content/drive/MyDrive/E-Commerce Tech Dataset/Dataset(Shophive HomeShopping PriceOye).csv`

## Requirements
The following Python libraries are required:
- `tensorflow`
- `pandas`
- `numpy`
- `matplotlib`
- `scikit-learn`

Install the dependencies using:
```bash
pip install tensorflow pandas matplotlib scikit-learn
```

## Usage
1. **Mount Google Drive**: Ensure the dataset is accessible by mounting Google Drive.
2. **Run the Notebook**: Execute the cells in the Jupyter Notebook to clean the data, train the model, and generate recommendations.
3. **View Recommendations**: The top 10 product recommendations will be displayed and saved to the dataset file.

## Key Functions
- **`clean_price(price)`**: Cleans the `product_price` column by removing unwanted characters and converting to numeric.
- **`clean_rating_count(rating_count)`**: Cleans the `rating_count` column by extracting numeric values.
- **`recommend_top_n(top_n=10)`**: Recommends the top N products based on predicted ratings.

## Outputs
- **Model Evaluation**: Displays the test loss and RMSE of the model.
- **Visualization**: A scatter plot comparing true and predicted ratings.
- **Recommendations**: A CSV file with the top N product recommendations.

## Example Output
Top 10 product recommendations:
```
                  product_name  predicted_ratings
1458         Realme 9 Pro Plus           0.579023
1465  Realme GT Master Edition           0.578578
182      Samsung Galaxy A53 5G           0.576258
1617            itel Value 110           0.573046
1610         E-Tachi B222 lite           0.572825
1673        Xiaomi Pad 5 Cover           0.572382
1508      Realme Dizo Star 300           0.571939
1653         Apple iPad mini 6           0.570744
1631            itel Muzik 410           0.570719
1632            itel Power 700           0.570603
```

## License
This project is licensed under the MIT License.
