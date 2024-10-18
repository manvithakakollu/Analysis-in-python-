#### Airbnb NYC Dataset Analysis
Overview
This repository contains an exploratory data analysis (EDA) of an Airbnb dataset focusing on properties available for short-term rental in New York City from 2011 to 2023. The dataset provides insights into various factors such as pricing, availability, and guest reviews across different neighborhoods and property types.

Dataset Description
The dataset consists of 42,931 entries and 18 columns, including:

id: Unique identifier for each property.

name: Name of the property.

host_id: Unique identifier for the host.

host_name: Name of the host.

neighbourhood_group: Boroughs of NYC (e.g., Manhattan, Brooklyn).

neighbourhood: Specific neighborhoods within the boroughs.

latitude: Latitude of the property location.

longitude: Longitude of the property location.

room_type: Type of accommodation (e.g., Entire home/apt, Private room).

price: Nightly price of the accommodation.

minimum_nights: Minimum stay requirement.

number_of_reviews: Total number of reviews received.

last_review: Date of the most recent review.

reviews_per_month: Average number of reviews per month.

calculated_host_listings_count: Total number of listings by the host.

availability_365: Number of available days in a year.

number_of_reviews_ltm: Number of reviews in the last twelve months.

license: Accommodation license (if applicable).

Special: Indicates if only one person has a license.

### Libraries Used
The analysis utilizes the following libraries:

pandas: For data manipulation and analysis.

numpy: For numerical computations.

seaborn and matplotlib: For data visualization.

missingno: To visualize missing data.

wordcloud: To create word clouds for text data.

plotly.express: For interactive visualizations.

#### Data Cleaning Process
Handling Missing Values:

Dropped the license column due to excessive NaN values.
Filled NaN values in reviews_per_month with its mode (0.02).

##Removing Duplicates:

Checked and removed duplicate entries from the dataset.

### Data Type Conversion:

Converted last_review to a datetime format.

Created a new column year from last_review for temporal analysis.

### Visualizations
The analysis includes various visualizations to explore:

Host listings count by room types and neighborhoods.

Price distribution by room type and neighborhood.

Heatmaps to visualize correlations between features.

Geographical distribution of properties using latitude and longitude.

Average price analysis by room type and neighborhood.
