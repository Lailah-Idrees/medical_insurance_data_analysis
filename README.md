# Medical Insurance Data Analysis

**Medical Insurance Data Analysis** is a comprehensive data analysis tool designed to streamline data exploration, analysis, and visualisation. The tool supports multiple data formats and provides an intuitive interface for both novice and expert data scientists.

# ![CI logo](https://codeinstitute.s3.amazonaws.com/fullstack/ci_logo_small.png)


## Dataset Content

This dataset contains medical insurance charges for individual policyholders, along with key demographic and lifestyle attributes such as age, BMI, sex, children, age and smoking status. The original dataset consists of 1,338 rows and 7 columns and was sourced from Kaggle link [here](https://www.kaggle.com/datasets/willianoliveiragibin/healthcare-insurance)

During the ETL phase of the data analysis process, additional features were created and added to the dataset. As a result, the final dataset includes the following columns:
* Age
* Sex
* bmi
* Weight_category
* Children
* Smoker
* Region
* Charges
* male_yes
* smoker_yes
* region_encoded


## Business Requirements
* In conducting analysis on fluctuations in medical insurance charges the business aims to understand they key factors that influence insurance charges across different customer groups. The business aims to identify patterns that drive higher or lower insurance costs through demographic and lifestyle analysis. This insight will support more accurate pricing strategies and ensure that insurance is aligned with customer needs


## Hypothesis and how to validate?
**Smokers will incur higher insurance charges across all combinations of demographic and lifestyle variables.**
* Use bivariate and multivariate visualisations that include smoking status as either an axis or a hue to compare charges across different groups and interactions.

**Women with children will pay more for insurance than men with children.**
* Create a multivariate boxplot for both men and women

**BMI is positively correlated with insurance charges — higher BMI leads to higher costs.**
* plot a scatterplot and a heatmap to check the correlation and how strong it is

**Smokers with a high bmi will incure the highest insurance charges overall.**
* facetted scatter plot one for smokers and one for non-snokers with  bmi and charges as the axis

**Gender does not significantly affect insurance charges.**
* Barplot and heat map

**Age is a strong predictor of insurance charges, with older individuals paying more.**

## Project Plan
1. Data Extraction 
* Find appropriate data from kaggle and download
* load data into project notebook and begin intial exploration
2. Data Cleaning
* Identify any null or empty values and discard and remove any dupliated data entries.
* Encode any categorical data using OneHotEncoder and Ordinal Encoder
* Outlier detection: remove outliers or use an appropriate transformer to reduce or remove outlier skewing effect
* Use boxplots to compare before and after transforming data to ensure the chosen technique worked
3. Load Data
* save cleaned dataset so it can be used across different notebooks
4. Data Visulisation
* Use MatPlotLib, Seaborn and plotly to visual and gain insights into the data in order to verify hypothesis and meet the business requirements
5. Report
* Summarise finding and draw a conclusion on the results

## The rationale to map the business requirements to the Data Visualisations
The primary business objective of this analysis is to understand what is driving the differences in insurance charges, to make sure they are fair and representative of individual circumstacne and to ensure all individual recieve the right cover.
* Identify key cost drivers
* Assess fairness across demographic group
* Ensure data quality for reliable insights
* Communicate findings clearly to stakeholders 
 Various techniques will be used to clean the data and make sure it is suitbale for visualisaton. Encoding and transformers will on categorical data and to remove outliers. When it came to visualtions plots from matoplotlib, seaborn and ploty were used to make sense of the data
## Analysis techniques used
* **Desciptive Statistics**
Used to get a general understanding of distribution of all numerical values
* Limitations: This technique cannot reveal relatioships between varibles

* **Correlation analysis (Scatter plots & Heatmaps)**
Used to map and quantify correlations between variable such as age, BMI, smoking status, Sex and number of children
* Limitation: correlation does not imply causation and only captures linear relationships

* **Data cleaning and preprocessing**

Included handling duplicates, encoding categorical variables, and preparing the dataset for analysis.
Limitation: The dataset was relatively small and lacked certain variables (e.g., income, occupation), which restricted the depth of analysis.

The analysis followed a progressive, layered structure:

**Data cleaning and preparation**  
Ensured the dataset was reliable and usable format before any insights were drawn.

**Bivariate analysis**
Examined relationships between pairs of variables (e.g., age vs charges, BMI vs charges).

**Multivariate exploration**
Used pairplots and grouped visualisations to understand how variables interact (e.g., smoker × BMI, sex × children).

**Hypothesis testing** 

AI is imbedded in the notebook so was used in an assistive way to fix error codes and explain how certain code blocks work.

## Ethical considerations
* Were there any data privacy, bias or fairness issues with the data? No
* How did you overcome any legal or societal issues?


## Unfixed Bugs
* No bugs detected 
* Did you recognise gaps in your knowledge, and how did you address them? When it came to formatting plot like subsetting them or isolating specific data to used in analysis was something i struggled with. I reviewed my notes and looked online for code to help


## Development Roadmap
* What challenges did you face, and what strategies were used to overcome these challenges? My vs code would crash or my git commit cycle wouldn't sync changes to my github repository. Overcoming this challeneges was farily simple i would use the built in git commit cycle instead
* What new skills or tools do you plan to learn next based on your project experience? becoming more efficient at finding solutions to coding errors


## Main Data Analysis Libraries
* pandas
Used for loading, cleaning, and preparing the dataset.

* matplotlib
Used to plot scatter plots, boxplots and histograms


* seaborn
Used for pairplots, heatmap and scatter plots. Helps with correlation analysis

* plotly
Used to build interactive charts such as the boxplot that compared gender with number of children and charges


## Credits 

* Data source from [here](https://www.kaggle.com/datasets/willianoliveiragibin/healthcare-insurance)
* Code for switching weight column can be found [here](https://saturncloud.io/blog/pandas-tips-reorder-columns/#:~:text=To%20move%20a%20column%20to,modifies%20the%20DataFrame%20in%2Dplace.&text=In%20summary%2C%20depending%20on%20the,columns%20to%20the%20desired%20order.)
* Code for displaying data in descending order can be found [here](https://github.com/DaniDL346/Global_Methane_Flux_Analysis/blob/main/README.md)

### Content 

- The text for the Home page was taken from Wikipedia Article A
- Instructions on how to implement form validation on the Sign-Up page was taken from [Specific YouTube Tutorial](https://www.youtube.com/)
- The icons in the footer were taken from [Font Awesome](https://fontawesome.com/)

### Media

- The photos used on the home and sign-up page are from This Open-Source site
- The images used for the gallery page were taken from this other open-source site



## Acknowledgements (optional)
* Thank the people who provided support through this project.