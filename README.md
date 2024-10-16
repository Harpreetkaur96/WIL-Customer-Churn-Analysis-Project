# WIL-Customer-Churn-Analysis-Project-
Stage 2 Deliverables: Data Preparation and Modeling
2-1: Data Preparation Deliverables:

A preprocessed dataset addressing missing data points and encoding categorical variables.
The dataset is split into distinct training and testing sets to facilitate model validation.
Appropriate scaling techniques are applied to normalize the data, enhancing model performance.
2-2: Clustering Analysis Deliverables:

The optimal number of clusters is identified using the elbow method.
A K-Means clustering model is trained on the dataset.
Resulting clusters are visualized and labeled for interpretation and actionable insights.
By completing these deliverables, the project team ensures the data is appropriately prepared and analyzed, setting the stage for effective modeling and predicting customer churn.

Data Preparation and Normalisation
1. Initial Data Overview:

Displays the structure and summary statistics of the dataset.
Helps in understanding the type and spread of data.
2. Handling Missing Values:

Missing values are handled using forward fill (df.fillna(method='ffill', inplace=True)), ensuring no gaps in data.
3. Encoding Categorical Variables:

Label encoding converts categorical variables into a numerical format suitable for machine learning models.
Sample display of the dataset post encoding shows the successful conversion.
4. Splitting Data:

The dataset is split into training (80%) and testing (20%) sets using train_test_split.
Ensures that the model can be validated on unseen data.
5. Scaling Data:

StandardScaler normalizes the feature set, standardizing it to have a mean of 0 and a variance of 1.
Ensures that features contribute equally to the model performance.
The scaled features are displayed to verify normalization.
Visual comparison of feature distribution before and after scaling ensures its effectiveness.
Clustering Analysis
1. Optimal Number of Clusters:

Elbow Method: The elbow plot indicates the optimal number of clusters (k). We plot SSE (Sum of Squared Errors) for a range of k values. The 'elbow' point, where the SSE begins to level off, suggests the optimal k. Here, k=4 appears to be optimal based on the plot.
Visualization: The elbow plot visually demonstrates how the SSE decreases with increasing k, guiding the choice of the optimal number of clusters.
2. Trained K-Means Model:

Training the Model: The K-Means model is trained using the optimal number of clusters (k=4). The code includes steps for training the model on the scaled data. -Saving the Model: The trained model is saved as a file (kmeans_model.pkl) for later use or deployment.
3. Visualization and Labeling of Clusters:

Adding Cluster Labels: Each data point is assigned a cluster label based on the trained model, and these labels are added to the dataset.
Cluster Visualization: The clusters are visualized using a scatter plot of 'tenure' vs. 'MonthlyCharges', colored by cluster labels. This visual representation helps interpret the clustering results, providing insights into the distribution and characteristics of different clusters.
3.1. Explanation of Visualizations

Elbow Plot: Helps determine the optimal number of clusters by showing where the rate of decrease in SSE slows significantly.
Cluster Visualization: Displays how data points are grouped into clusters, aiding in the identification of patterns and insights related to customer churn.
