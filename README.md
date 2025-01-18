# Taxi_rides_EDA_SQL_S6

# README: Taxi Rides Data Analysis and Hypothesis Testing

---

## Project Overview
This project analyzes taxi ride data in Chicago to uncover insights about taxi company performance, drop-off patterns, and ride durations under specific conditions. It involves exploratory data analysis (EDA) and hypothesis testing using Python.

---

## Data Sources
### CSV Files Provided:
1. **`/datasets/project_sql_result_01.csv`**  
   - `company_name`: Taxi company name  
   - `trips_amount`: Number of rides on November 15-16, 2017  

2. **`/datasets/project_sql_result_04.csv`**  
   - `dropoff_location_name`: Chicago neighborhoods where rides ended  
   - `average_trips`: Average number of rides that ended in each neighborhood in November 2017  

3. **`/datasets/project_sql_result_07.csv`**  
   - `start_ts`: Pickup date and time  
   - `weather_conditions`: Weather conditions at the ride's start time  
   - `duration_seconds`: Ride duration in seconds  

---

## Steps to Complete the Project

### Step 1: Data Import
- Load the datasets into Python using `pandas`.

### Step 2: Data Exploration
- Inspect the data for completeness, consistency, and correctness.
- Ensure proper data types for each column.

### Step 3: Data Analysis
1. **Dataset 1 (`project_sql_result_01.csv`):**
   - Analyze taxi companies and the number of rides.
   - Visualize the number of rides for each taxi company using a bar graph.

2. **Dataset 2 (`project_sql_result_04.csv`):**
   - Identify the top 10 neighborhoods with the highest number of drop-offs.
   - Create a bar graph to visualize the drop-offs in these neighborhoods.

3. **Insights and Conclusions:**
   - Summarize findings based on the visualizations, such as identifying high-performing taxi companies and popular drop-off areas.

### Step 4: Hypothesis Testing
- Use `project_sql_result_07.csv` to test the hypothesis:  
  **"The average duration of rides from the Loop to O'Hare International Airport changes on rainy Saturdays."**

1. **Formulate Hypotheses:**
   - Null Hypothesis (\(H_0\)): The average ride duration on rainy Saturdays is the same as on non-rainy Saturdays.  
   - Alternative Hypothesis (\(H_a\)): The average ride duration on rainy Saturdays differs from non-rainy Saturdays.

2. **Set the Significance Level:**
   - Decide on an alpha value (e.g., 0.05).

3. **Select Statistical Test:**
   - Use a two-sample t-test for comparing mean ride durations under the two conditions. Ensure assumptions for the t-test are met.

4. **Perform the Test:**
   - Conduct the test using `scipy.stats`.
   - Analyze the p-value to accept or reject the null hypothesis.

5. **Conclude:**
   - Summarize the findings and their implications.

---

## Dependencies
- Python 3.x  
- Libraries: `pandas`, `matplotlib`, `seaborn`, `scipy`

---

## Execution
1. Clone this repository or download the datasets.
2. Install required dependencies.
3. Run the Jupyter Notebook or Python script provided with the project.
4. Review the results and visualizations.
