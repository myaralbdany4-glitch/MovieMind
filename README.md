 MovieMind: AI-Powered Movie Recommendation System

## 1. Load and Explore
I used the **MovieLens (ml-latest-small)** dataset. After merging the ratings and movies files, I explored the data structure. I identified a **class imbalance**, where positive ratings were more frequent than negative ones. Therefore, I chose the **F1-score** as my primary metric.

## 2. Prepare the Data
I performed **Feature Engineering** by extracting the "Year" and calculating the "Average Rating" for each movie. I categorized ratings into: **Liked, Neutral, and Not Liked**. The data was split into **80% training** and **20% testing**.

## 3. Train and Compare Models
I trained three models: **Logistic Regression, Random Forest, and KNN**. 
* **Random Forest** performed best due to its ability to handle complex non-linear relationships in the movie data.

## 4. Neural Network Build and Train
I built a Deep Learning model using **Keras** with **Dense layers** and **ReLU** activation. I added a **Dropout layer (30%)** to prevent overfitting and trained it for 10 epochs.

## 5. Comparison and Results
After evaluation, the **Random Forest** and **Neural Network** showed the highest performance. I selected the best model based on the weighted F1-score to ensure accuracy across all rating classes.

## 6. Conclusion
The project successfully demonstrates how machine learning can predict user preferences. Adding custom features like "average movie rating" was the key to improving the system's accuracy.
