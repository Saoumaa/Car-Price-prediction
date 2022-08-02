# Car-Price-prediction

This is based on the prediction of price of cars. It is also a regression problem. 
## Importing Libraries.
since this is a small one, few libraries were imported. The imported libraries include:
1. pandas
2. seaborn
3. matplotlib.pyplot
4. sklearn and its functions

## Loading the dataset
The dataset was loaded using panadas.
The dataset have 301 rows and 9 columns (inclusing the price column). The dataset contains both numerical and categorical features.
From the description of the data, it can be seen that there are outilers in the data (there is a large gap between the 75 percentile and 100 percentile of the data.)

## Data Visualization
To visualize the data, seaborn was used.
The visualization of the categorical type data is shown below:

#### Fuel Type
![download](https://user-images.githubusercontent.com/104036386/182394061-77f26fec-ebe3-4d74-8761-d5ea7c3ee9bb.png)

#### Owner
![download](https://user-images.githubusercontent.com/104036386/182394137-729edee6-8ff0-499e-8789-a9180f3f4669.png)

#### Year
![download](https://user-images.githubusercontent.com/104036386/182394185-422a3242-fea1-4da9-affa-c36351b1163d.png)

#### Seller Type
![download](https://user-images.githubusercontent.com/104036386/182394298-9666e0f2-2615-4a7f-bb49-ff657a96ebad.png)

#### Transmission
![download](https://user-images.githubusercontent.com/104036386/182394426-23ff995d-11f2-46b7-8f77-84f69162a3a8.png)

## Categorizing the data
Here, the categorical type data were categorized. To do this, pandas dummies were used to transform the categorical data.

##### Note that the ourliers weren't removed, the reason for this is because of the small size of the data. Machine learning models needs a large amount of data to properly fit the training sets. Hence they were not removed.

## Modeling

The first model used is CatBoostRegressor, followed by

#### CatBoosRegressor
This model produced an accuracy of 94%

#### Linear Regressor
This model achieved an accuraccy of 85%

#### GradientBoostingRegressor
This model achieved an accuracy of 93%

#### RandomForestRegressor
This model achieved an accuracy of 92%

The model that performed best so far is the CatBoostRgressor.
With this model, the prediction made have a 94% rate of being the exact one.
