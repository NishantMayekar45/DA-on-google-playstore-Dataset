
#Data Analysis on Google PlayStore Dataset

While many public datasets (on Kaggle and the like) provide Apple App Store data, there are not many counterpart datasets available for Google Play Store apps anywhere on the web. On digging deeper, I found out that iTunes App Store page deploys a nicely indexed appendix-like structure to allow for simple and easy web scraping. On the other hand, Google Play Store uses sophisticated modern-day techniques (like dynamic page load) using JQuery making scraping more challenging.

In this Notebook, we cleaned the dataset by implementing Data Pre-processing and Analyzed in order to gain insights from it.

The dataset is collected from kaggle: Link

Dataset Description -
App - Application name
Category - Category the app belongs to
Rating Overall - user rating of the app (as when scraped)
Reviews - Number of user reviews for the app (as when scraped)
Size - Size of the app (as when scraped)
Installs - Number of user downloads/installs for the app (as when scraped)
Type - Paid or Free
Price - Price of the app (as when scraped)
Content Rating - Age group the app is targeted at Children / Mature 21+ / Adult
Genres - An app can belong to multiple genres (apart from its main category). For eg, a musical family game will belong to Music, Game, Family genres.
Last Updated - Date when the app was last updated on Play Store (as when scraped) Current version of the app available on Play Store (as when scraped)
Current Ver - Current Android Version
Android Ver - Min required Android version (as when scraped)
The main tasks performed in this jupyter notebook are -
Data Analysis
Data Cleaning
Data Pre-processing
Data Visualisation
Methodologies -
We will perform the following steps for Data Cleaning and Data Preparation -

Deal with missing values and ‘Varies with device’ data.
Removing characters from Installs and make it numeric.
Remove ‘M’(megabyte) from the size and make it numeric.
Remove ‘k’(kilobyte) from size, make it numeric then divide it by 1000.
Transform reviews to numeric.
Remove currency symbol from Price, change it to numeric
Convert ‘Last Updated’ date to date format
Round current version number to 1 decimal
