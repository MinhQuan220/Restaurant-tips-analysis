# **🍽️ Restaurant Tips Analysis**

## 1. A brief description of what your project does

This project aims to use the restaurant tips dataset to practice creating composition plots and visualizations. We will examine the relationship between different variables and the tips given.

The dataset consists of information from 244 restaurant bills, collected in the US in 1987.

It includes details about the tips given to restaurant staff, such as the total bill, tip amount, gender of the person paying, smoking status, day of the week, time of day, and party size.
 ![image](https://thietbikhachsancomvn.wordpress.com/wp-content/uploads/2021/02/nha-hang-la-gi1.jpg?w=1000)
 
## 2. 📥 Data import

First, let's import the needed libraries: Pandas & Matplotlib

```Python
import pandas as pd
import matplotlib.pyplot as plt
```
Then load data from the following link: https://raw.githubusercontent.com/RusAbk/sca_datasets/main/tips.csv
```Python
df = pd.read_csv('https://raw.githubusercontent.com/RusAbk/sca_datasets/main/tips.csv')
```
### 2.1 🔍 Data exploration

#### 2.1.1 Test sample
A quick look at the first few rows (df.head()) confirms that the data was loaded correctly and provides a first glimpse of the columns and their structure.
```Python
df.head()
```

#### 2.1.2 Column types checking
Show the columns of the dataframe and their types:
```Python
df.info()
```

#### 2.1.3 Basic descriptive statistics
Descriptive statistics (`df.describe()`) were generated for the numerical columns (`id`, `total_bill`, `tip`, `size`) to understand their central tendency, dispersion, and range.

## 3. The main goals
The main goals of this analysis were to investigate how different factors influence the tip amount. Specifically, the project explored the impact of:

*   Smoking status (Smokers vs. Non-smokers)
*   Gender (Males vs. Females)
*   Day of the week (Weekdays vs. Weekends)
*   Time of day (Lunch vs. Dinner)

## 4. Results

*   Smoking status (Smokers vs. Non-smokers)
  ![image](<img width="839" height="275" alt="{F531A22C-7662-4697-98B3-796D493257ED}" src="https://github.com/user-attachments/assets/528b5355-1fd4-475d-896a-7de57dc7ae89" />)

*   Gender (Males vs. Females)
*   Day of the week (Weekdays vs. Weekends)
*   Time of day (Lunch vs. Dinner)
  
## 5.Conclusions
The analysis involved separating the data based on the influencing factors, comparing the measures of central tendency (min, max, mean, median) for the tip amounts in each group, and visualizing the tip distributions using histograms with median lines for comparison.

Key findings include:

*   **Smoking Status:** Smokers tend to give slightly higher average and median tips than non-smokers, although the overall difference is not large. The distribution for smokers shows a slightly wider spread towards higher tips.
*   **Gender:** Males tend to give higher average and median tips compared to females. Notably, males also have a higher potential for exceptionally high tip amounts than females in this dataset.
*   **Day of the Week:** Weekends (Saturday and Sunday), particularly Sunday, tend to yield higher average and median tips than weekdays (Thursday and Friday). The possibility of receiving very large tips is also higher on weekends, especially on Saturday.
*   **Time of Day:** Dinner service generally receives significantly higher average and median tips and has a greater potential for larger individual tips compared to lunch service.

These results provide insights into the factors that correlate with higher tip amounts in this specific restaurant dataset.
