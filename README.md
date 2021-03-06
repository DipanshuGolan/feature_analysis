# Feature Analysis: Simple Feature Analysis in Python

It performs feature analysis for data preprocessing or usage of data in Machine Learning.
# Methods

There are four methods used to identify features to remove:

1. Finding Missing Values (find_missing(missing_threshold)) 

   %% Find the features with a fraction of missing values above `missing_threshold`
2. Single Unique Values (find_unique())

    %% Find the features having a single unique value. NaNs do not count as a unique value.
3. Collinear Features (find_collinear(correlation_threshold,one_hot=False))

   %% Finds collinear features based on the `correlation coefficient` between features.
4. Low Importance Features (find_low_impt(cumulative_impt,label))

   %% Finds the lowest importance features not needed to account for `cumulative_importance` fraction
        of the total feature importance from the gradient boosting machine.
        label corresponding to regession or classification

## Usage

Refer to the [testing.py](https://github.com/DipanshuGolan/feature_analysis/blob/main/testing.py) for how to use the different methods in module.

## Visualizations

The `FeatureAnalysis` methods also includes a number of visualization in each methods mentioned above to inspect 
characteristics of a dataset. 

### Histogram for missing values
![](images/Figure_1.png)

### Histogram for unique values
![](images/Figure_2.png)

### Correlation Heat map
![](images/Figure_3.png)

### Important Features
![](images/Figure_4.png)

### Cumulative Feature Importance
![](images/Figure_5.png)

# Requirements:
Install dependencies just mentioned in requirements.txt by typing command in shell.

`pip install -r requirements.txt`

## Contact

Any questions can be directed to dipanshugolan96@gmail.com.

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.
