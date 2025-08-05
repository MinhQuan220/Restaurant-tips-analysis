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
Take a look at the first 5 rows to be sure, that data is loaded properly:
```Python
df.head()
```
 ![image](<img width="549" height="230" alt="{BA21C211-90FD-4C33-A261-9388390A0264}" src="https://github.com/user-attachments/assets/29178072-50f2-49c1-9589-afb191ca3414" />)

#### 2.1.2 Column types checking
Show the columns of the dataframe and their types:
```Python
df.info()
```

#### 2.1.3 Basic descriptive statistics
## 3. The main goals
## 4. Results
