# Taxi_rides_EDA_S6

# Taxi Rides Data Analysis and Hypothesis Testing

---

## Project Overview
This project analyzes taxi ride data in Chicago to uncover insights about taxi company performance, drop-off patterns, and ride durations under specific conditions. It involves exploratory data analysis (EDA) and hypothesis testing using Python.

---

## Data Sources
### CSV Files Provided:
1. **`/datasets/project_sql_result_01.csv`**  
   - `company_name`: Taxi company name  
   - `trips_amount`: Number of rides on November 15–16, 2017  

2. **`/datasets/project_sql_result_04.csv`**  
   - `dropoff_location_name`: Chicago neighborhoods where rides ended  
   - `average_trips`: Average number of rides ending in each neighborhood in November 2017  

3. **`/datasets/project_sql_result_07.csv`**  
   - `start_ts`: Pickup date and time  
   - `weather_conditions`: Weather conditions at the start of the ride  
   - `duration_seconds`: Ride duration in seconds  

---

## Steps to Complete the Project

### Step 1: Data Import
- Load the datasets into Python using `pandas`.

### Step 2: Data Exploration
- Inspect the data for completeness, consistency, and correctness.
- Ensure proper data types are assigned to each column.

### Step 3: Data Analysis
- **Dataset 1 (`project_sql_result_01.csv`):**  
  - Analyze taxi companies and their number of rides.
  - Create a bar graph to visualize the number of rides per taxi company.

- **Dataset 2 (`project_sql_result_04.csv`):**  
  - Identify the top 10 neighborhoods with the highest number of drop-offs.
  - Create a bar graph to visualize the drop-offs in these neighborhoods.

- **Insights and Conclusions:**  
  - Summarize key findings based on the visualizations, including high-performing companies and popular drop-off locations.

### Step 4: Hypothesis Testing
Using `project_sql_result_07.csv`, test the hypothesis:

> **"The average duration of rides from the Loop to O'Hare International Airport changes on rainy Saturdays."**

- **Formulate Hypotheses:**  
  - Null Hypothesis (\(H_0\)): The average ride duration on rainy Saturdays is the same as on non-rainy Saturdays.  
  - Alternative Hypothesis (\(H_a\)): The average ride duration on rainy Saturdays is different from non-rainy Saturdays.

- **Set the Significance Level:**  
  - Use an alpha value of 0.05.

- **Select the Statistical Test:**  
  - Perform a two-sample t-test to compare mean ride durations between the two conditions.  
  - Check that the assumptions for the t-test are satisfied.

- **Conduct the Test:**  
  - Use `scipy.stats` to perform the test.
  - Analyze the p-value to determine whether to reject the null hypothesis.

- **Conclude:**  
  - Summarize the results and their practical implications.

---

## Dependencies
- Python 3.x  
- Libraries: `pandas`, `matplotlib`, `seaborn`, `scipy`

---

## Execution
1. Clone this repository or download the datasets.
2. Install the required dependencies.
3. Run the provided Jupyter Notebook or Python script.
4. Review the results and visualizations.
