# Day 1: Data Preprocessing 

### Important Libraries
  - Numpy: Support for large multi-dimensional arrays and hosts a large collections of high-level math function that can be used to operate on arrays.
  - Pandas: Data analysis and manipulation tool for working with relational and labeled data
  - Scikit-learn: Machine learning library
  ```
  pip install pandas
  pip install numpy
  pip install scikit-learn
  ```
### What is data pre-processing?
  
It is the technique of cleaning and oragnizing raw data to make it suitable for building and training machine learning models
  
### Data Cleaning
  
We want to be able to calibrate datasets to account for real world occurances such as incomplete/missing values, noise, and inconsistencies. 

  - Missing Values
    - Common Practice is to fill in the missing value with the average/mean
    - SimpleImputer finds all NaN values in a column and replaces them with the mean

  - Encoding categorical Data
    - Types of data which can be divided in to groups. Ex : sex and race
    - LabelEncoder transforms values to the integer representation  
 
### Training and Test datasets
 
