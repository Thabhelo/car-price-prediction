# Car Price Prediction Data Analysis

This project involves analyzing a car price dataset using Python libraries such as NumPy, Pandas, Matplotlib, Seaborn, and sklearn. The goal is to pre-process the dataset by applying feature engineering, feature selection, and exploratory data analysis. Note that actual model building is not part of this project.

## Table of Contents
- [Project Description](#project-description)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Analysis Steps](#analysis-steps)
  - [Section 1: Data Types and Preprocessing](#section-1-data-types-and-preprocessing)
  - [Section 2: Data Cleaning and Exploration](#section-2-data-cleaning-and-exploration)
  - [Section 3: Feature Engineering and Encoding](#section-3-feature-engineering-and-encoding)
  - [Section 4: Feature Selection Based on Correlation](#section-4-feature-selection-based-on-correlation)
  - [Section 5: Feature Selection Using SelectKBest](#section-5-feature-selection-using-selectkbest)
- [Conclusions](#conclusions)
- [Contributing](#contributing)
- [License](#license)

## Project Description

The goal of this project is to analyze a car price dataset and perform various data preprocessing tasks, including feature engineering, feature selection, and exploratory data analysis. This analysis will help develop machine learning models that can accurately predict car prices based on various features such as model, production year, category, brand, fuel type, engine volume, mileage, cylinders, vehicle style, and others.

## Dataset

The dataset consists of 19,237 samples and includes features such as:

- Model
- Production year
- Category
- Brand
- Fuel type
- Engine volume
- Mileage
- Cylinders
- Vehicle style
- Price (target variable)

## Installation

To run this project, you'll need to install the following dependencies:

- Python 3.x
- NumPy
- Pandas
- Matplotlib
- Seaborn
- scikit-learn
- Jupyter Notebook

You can install the required packages using pip:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn jupyter
```

## Usage

```bash
git clone https://github.com/yourusername/car-price-prediction.git
```
```bash
cd car-price-prediction
```
```bash
python -m venv envsource env/bin/activate # On Windows use \`env\\Scripts\\activate\`
```
```bash
pip install numpy pandas matplotlib seaborn scikit-learn jupyter
```
```bash
jupyter notebook
```
Open **car\_price\_analysis.ipynb** and run the cells sequentially to perform the data analysis.
    

## Project Structure


The project directory contains the following files:

*   **car\_price\_analysis.ipynb**: The Jupyter Notebook containing the data analysis and preprocessing steps.
    
*   **price_prediction_batch_23.csv**: The dataset used for the analysis.
    
*   **README.md**: The project documentation.
    

## Analysis Steps

### Section 1: Data Types and Preprocessing

*   Analyze data types of features and update if required.
    
*   Process the 'Levy' column and convert it to an integer type.
    
*   Process the 'Mileage' column and convert it to an integer.
    
*   Check for NaN values in the data and remove them if necessary.
    

### Section 2: Data Cleaning and Exploration

*   Check for duplicates and remove them.
    
*   Check for outliers using boxplots and statistical methods, and remove them if necessary.
    
*   Draw countplots for categorical features and write observations.
    
*   Draw histograms for numeric features, compute skewness, and apply transformation functions if needed.
    

### Section 3: Feature Engineering and Encoding

*   Create a joint plot with the hue parameter and write observations.
    
*   Apply scaling methods to independent features.
    
*   Convert categorical features into numeric ones using appropriate encoding techniques.
    
*   Combine results and compute the correlation among all independent features using a heatmap. Discard one of the variables if high correlation is detected (above 0.7).
    

### Section 4: Feature Selection Based on Correlation

*   Split the dataset into training and testing sets using an 80-20 split.
    
*   Compute the correlation of each independent feature with the dependent variable 'Price'.
    
*   Select the seven most important independent features based on the correlation values.
    

### Section 5: Feature Selection Using SelectKBest

*   Apply the **SelectKBest** method to the dataset to reduce the feature set to the seven most important features.
    

## Conclusions

*   The analysis identified key features influencing car prices and reduced the feature set to the most relevant ones for potential model building.
    
*   Data preprocessing steps, including handling missing values, outliers, and feature scaling, were crucial in preparing the data for analysis.
    

## Contributing

Contributions are welcome! Please fork this repository and submit a pull request for any enhancements or bug fixes.

## License

This project is licensed under the MIT License. See the LICENSE file for details.
