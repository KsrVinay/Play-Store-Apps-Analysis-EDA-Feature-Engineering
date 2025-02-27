# 📊 Play Store EDA and Feature Engineering  

## 📌 Overview  
This project involves **Exploratory Data Analysis (EDA)** and **Feature Engineering** on the **Google Play Store dataset**. The dataset contains information about various apps available on the Play Store, including:  
- App name  
- Category  
- Rating  
- Reviews  
- Installs  
- Type (Free/Paid)  
- Price  
- Content rating  
- Last updated date  
- Android version  

The goal of this project is to **clean, analyze, and transform** the dataset to extract meaningful insights and prepare it for further **machine learning tasks**.  

## 📂 Dataset  
The dataset used in this project is **googleplaystore.csv**, which contains **10,841 rows** and **13 columns**. The columns include:  

- **App**: Name of the application  
- **Category**: Category to which the app belongs  
- **Rating**: User rating of the app  
- **Reviews**: Number of user reviews  
- **Size**: Size of the app  
- **Installs**: Number of installs/downloads  
- **Type**: Free or Paid  
- **Price**: Price of the app  
- **Content Rating**: Target audience for the app  
- **Genres**: Genre of the app  
- **Last Updated**: Date when the app was last updated  
- **Current Ver**: Current version of the app  
- **Android Ver**: Minimum Android version required  

## 🔍 Project Steps  

### 1️⃣ Data Loading and Initial Inspection  
- **Libraries Used**: `numpy`, `pandas`, `matplotlib`, `seaborn`  
- **Data Loading**: The dataset is loaded using `pandas.read_csv()`  
- **Initial Inspection**: Used `.head()`, `.shape`, `.info()`, and `.describe()` to understand the structure and summary statistics  

### 2️⃣ Data Cleaning  
- **Handling Missing Values**: Identified and handled missing values in `Rating`, `Type`, `Content Rating`, `Current Ver`, and `Android Ver`  
- **Removing Duplicates**: Dropped duplicate rows and duplicate app names  
- **Data Type Conversion**: Converted `Reviews`, `Size`, `Installs`, and `Price` to appropriate data types  
- **Date Parsing**: Extracted day, month, and year from the `Last Updated` column  

### 3️⃣ Feature Engineering  
- **Size Conversion**: Converted `Size` column to a uniform format (MB)  
- **Installs Conversion**: Cleaned `Installs` column by removing commas and plus signs, converting it to integer values  
- **Price Conversion**: Cleaned `Price` column to remove dollar signs and converted it to float values  
- **Date Features**: Extracted day, month, and year from `Last Updated`  

### 4️⃣ Exploratory Data Analysis (EDA)  
- **Univariate Analysis**: Used histograms and box plots to understand the distribution of numerical columns  
- **Handling Outliers**: Identified and handled outliers in numerical columns  
- **Categorical Analysis**: Analyzed `Category`, `Type`, and `Content Rating`  

### 5️⃣ Data Visualization  
- **Histograms and Box Plots**: Visualized the distribution of numerical columns  
- **Bar Charts**: Visualized the distribution of categorical columns  
- **Scatter Plots**: Explored relationships between different numerical features  

### 6️⃣ Saving the Cleaned Dataset  
- The **cleaned and transformed dataset** is saved as `cleaned_googleplaystore.csv` for further use in **machine learning models**.  

## 📈 Key Insights  
✔ **Missing Values**: Identified and handled missing values in multiple columns  
✔ **Data Cleaning**: Ensured data consistency by converting columns to appropriate data types  
✔ **Feature Engineering**: Created new features like `Last Updated_day`, `Last Updated_month`, and `Last Updated_year`  
✔ **Visualization**: Provided visual insights into the dataset’s distribution and relationships  

## ✅ Conclusion  
This project successfully **cleaned and transformed** the **Google Play Store dataset**, making it **ready for further analysis and machine learning tasks**. The **EDA provided valuable insights** into the distribution of apps, their ratings, installs, and other key features. The cleaned dataset can now be used to build **predictive models** or perform **advanced analytics**.  

## 🔮 Future Work  
🚀 **Machine Learning Models**: Use the cleaned dataset to build predictive models for app ratings or installs  
🚀 **Advanced EDA**: Perform deeper analysis to uncover hidden insights and relationships  
🚀 **Feature Selection**: Identify the most important features for predicting app success  
