# Crime Data Analysis and Visualization

This project analyzes crime data across different states, with a focus on crime categories such as Fraud, Extortion, and others. The analysis includes descriptive statistics, correlation analysis, and visualizations such as stacked bar charts, heatmaps, and pie charts. It aims to provide insights into crime patterns and trends across states, helping to understand the distribution and relationship between different crime types.

## Features
**Descriptive Statistics**: Provides a summary of the dataset including central tendency, dispersion, and distribution.
**Correlation Analysis**: Analyzes the relationships between different crime categories using Pearson correlation.
**Crime Distribution**: Visualizations such as stacked bar charts and pie charts to show the distribution of crimes by type and by state.
**State Crime Ranking**: A bar chart showing states ordered by the total number of offenses.
**Crime Proportions**: A pie chart showing the distribution of different crime types across all states.

## Technologies Used
**Python**: Programming language used for data analysis.
**Pandas**: Library for data manipulation and analysis.
**Seaborn**: Library for data visualization, particularly for statistical plots.
**Matplotlib**: Library for creating static, animated, and interactive visualizations.
**Scikit-learn**: Used for standard scaling and modeling tasks (though not used directly in the given code).

## Code Example

```python
import pandas as pd
from sklearn.preprocessing import StandardScaler
import seaborn as sns
import matplotlib.pyplot as plt
from sklearn.model_selection import train_test_split
from sklearn.linear_model import LinearRegression
```
## Installation Instructions

### Requirements:
1. Python 3.7 or later
2. Pip for installing pandas,seaborn,matplotlib,scikit-learn
### Steps:
1. Clone the repository:
    ```bash
    git clone https://github.com/Kavana89/crime-data-analysis.git
    cd crime-data-analysis
    ```

2. Install the required dependencies:
    ```bash
    pip install pandas,seaborn,matplotlib,scikit-learn
     ```

3. Ensure the dataset (CSV file) is present in the specified directory (for example, `"C:\\Users\\kavan\\OneDrive\\Documents\\state.csv"`). 

4. Run the Python script:
    ```bash
    python crime_analysis.py
    ```

    This will display various visualizations including correlation heatmaps, bar charts, and pie charts based on the crime data.

## How it Works

### Data Preprocessing:
The dataset is first loaded into a pandas DataFrame.
Rows and columns with all-zero values are removed to ensure meaningful analysis.
The `State` column is excluded from correlation analysis, as it's categorical.
  
### Analysis and Visualization:
1. **Descriptive Statistics**: A summary of the dataset is generated using `df.describe()`, which provides central tendency (mean, median), dispersion (standard deviation), and the shape of distributions.
2. **Correlation Analysis**: Pearson correlation coefficients between the numeric crime categories are calculated to identify relationships between different types of crimes.
3. **Visualizations**:
   **Heatmap**: A correlation heatmap to visualize the relationships between different crime categories.
   **Stacked Bar Chart**: A chart comparing crime counts across states for each crime type.
   **Total Crimes by State**: A bar chart showing the states ordered by total crime counts.
   **Crime Proportions**: A pie chart showing the proportion of each crime type across all states.

## Sample Outputs

1. **Correlation Heatmap**: A heatmap to visualize correlations between crime categories.
2. **Stacked Bar Chart**: A stacked bar chart comparing crime counts across states.
3. **Total Crimes by State**: A bar chart ranking states by total number of crimes.
4. **Crime Proportions**: A pie chart showing the proportions of each crime type.

## Dataset

The dataset used in this project contains information on various crime types across different states. The dataset is assumed to be in a CSV format with the following structure:

- **State**: The name of the state.
- **Crime Categories**: Columns representing different crime types such as 'Fraud', 'Extortion', 'Prank', etc.
  
### Sample CSV Structure:
| state        | Fraud | Extortion | Prank | ... |
|--------------|-------|-----------|-------|-----|
|Andhra Pradesh| 537   | 65        | 0     | ... |
|ArunachalPradesh| 0   | 0         | 0     | ... |
|Assam         | 48    | 65        | 40    | ... |
| ...          | ...   | ...       | ...   | ... |

