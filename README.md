#       udacity-Airbnb Boston , NY


I want to thank udacity for providing me this opportunity to write a  data science blog post on analysis of airbnb homes in ny boston
THE project follows CRIPS DM process 
The readme contains a go through of the projet.

1> Business Understanding
2> Data Understanding
3>Data PRepration 
4> Modelling
5> Evaluation
#      LIBRARIES
The following libraries were used in the development of the project:
numpy
 pandas 
 matplotlib.pyplot
 sklearn.linear_model
klearn.model_selection,  train_test_split
sklearn.metrics 
 seaborn 
 
 #      MOTIVATION : 
 Airbnb is a popular housing rental site  , the data set for Boston City contains a lot of columns and information thorugh which various inferences and shortcomings can be   drawn to further improve the business model. I undertook this project due to the huge amount of data the set contains and the various scope it has in analysing the various aspects of it .

The Repository contains 3 files :

1. DSProject.ipynb : 
   Python file which contains all the data anlysis modelling and visualisation of the Airbnb Listings data set
2.listings.csv : 
  Csv file containing information on the information of various listings spread across the city of Boston ,Ny
3. Readme.md :
  Readme contains the go through of the project motivation and various libraries used in the the project.
 


!> Business Understanding : 
The main focus of this project is to check what affects the superhost and what affects the price?
How well we can predict the price and check what factors strongly relate with the superhost

2>Data Understanding :
 The data contains 3 Datasets mainly calendar listings and reviews. We have explored listings dataset.
 The listings data set contains 3585 rows and 95 columns
 Columns with 75 % missing values are :
{'has_availability', 'square_feet', 'neighbourhood_group_cleansed', 'weekly_price', 'license', 'jurisdiction_names', 'monthly_price'}

2> DAta PRepration :
WE see that many columns contain special characters, NAn values  The data is filtered for the same and used in the training of the model
The following list contains columns with their Nan values respectively
id 0
scrape_id 0
host_id 0
host_response_rate 471
host_acceptance_rate 471
host_listings_count 0
host_total_listings_count 0
neighbourhood_group_cleansed 3585
latitude 0
longitude 0
accommodates 0
bathrooms 14
bedrooms 10
beds 9
square_feet 3529
price 0
weekly_price 2693
guests_included 0
minimum_nights 0
maximum_nights 0
has_availability 3585
availability_30 0
availability_60 0
availability_90 0
availability_365 0
number_of_reviews 0
review_scores_rating 813
review_scores_accuracy 823
review_scores_cleanliness 818
review_scores_checkin 820
review_scores_communication 818
review_scores_location 822
review_scores_value 821
license 3585
jurisdiction_names 3585
calculated_host_listings_count 0
reviews_per_month 756

2. THe amenities in any room are an important aspect of the quality of the hotel.
 THe amenities are stored in a separate list and checked with host_is_superhost with their correlation

3. What kind of reviews affect the capability of a host to be a superhost 
 Some basic data exploration is done on the price and other  types of houses
We find that for amenities Parking has the strongest correlation with superhosts 
Whereas for Reviews values and review ratings

#      MODELLING :

THe data is split into train and test data with 70  % and 30 % split
The model used is linear regression model with random state of 42
Te r squared value on training data was 0.319 while on test data was 0.229






