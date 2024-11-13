# IPL_Auction_Data_Analysis-_2022

## Overview
This project conducts an exploratory data analysis (EDA) of the 2022 IPL (Indian Premier League) auction dataset. Through this analysis, the project aims to uncover insights regarding player retention, purchase trends, and team-wise acquisitions, along with the cost dynamics in the auction. The project leverages data manipulation and visualization techniques to draw meaningful conclusions about player acquisitions and spending patterns by IPL teams.

## Objective
The primary goal of this project is to analyze the 2022 IPL auction data to:
- Understand the distribution of sold and unsold players across teams.
- Examine the player retention and acquisition strategies of each team.
- Identify the highest spending teams and analyze costs associated with top players.
- Generate actionable insights into the types of players (bowlers, batsmen, all-rounders, etc.) preferred by various teams.

## Project Execution

### 1. Data Loading and Libraries
- **Tools & Libraries**: Python, Pandas, NumPy, Matplotlib, Seaborn
- Imported the dataset `ipl_2022_dataset.csv` using Pandas and loaded essential libraries for analysis.

### 2. Data Cleaning and Preprocessing
- **Initial Exploration**: Assessed dataset structure, data types, and null values using `.info()` and `.head()` functions.
- **Null Value Handling**: Replaced missing values in key columns:
  - `COST IN ₹ (CR.)` and `Cost IN $ (000)` were filled with 0.
  - Null values in `2021 Squad` were filled with 'Not Participated.'
- **Column Management**: Dropped unnecessary columns such as the `Unnamed: 0` index column to streamline data analysis.

### 3. Exploratory Data Analysis (EDA)

- **Sold vs. Unsold Players**:
  - Analyzed and visualized the sold vs. unsold status of players using a bar plot, with `237` players marked as "sold" and `396` as "unsold."
  - Added a `status` column to classify players as 'sold' if they were associated with any team.

- **Player Types**:
  - Examined the distribution of different player types (batsman, bowler, all-rounder, wicketkeeper) using a pie chart, identifying team preferences.

- **Team-Based Analysis**:
  - Analyzed the total number of players acquired by each team and visualized this using a bar graph, highlighting team-specific acquisition strategies.
  - Compared the distribution of different player types in each team to understand team dynamics and preferences.

### 4. Advanced Analysis and Insights

- **Cost and Retention Analysis**:
  - Created a `retention` column, categorizing players based on whether they were retained, auctioned, or draft-picked.
  - Extracted price details in `base_price` and `base_price_unit` to compare the auction costs and base prices of different players.

- **Team-Wise Spending**:
  - Analyzed the highest costs paid per player for each team. For instance, Mumbai Indians spent a maximum of 15.25 Cr on a single player.
  - Identified the top 5 highest-cost bowlers and assessed the premium pricing for key players.

- **Unsold Players Analysis**:
  - Listed key unsold players from each team in the previous season, such as Suresh Raina (CSK) and Steve Smith (DC), and analyzed possible reasons for their unsold status.

## Key Findings

- **Sold vs. Unsold**: Approximately 63% of players remained unsold, indicating high competition among players for team slots.
- **Team Strategies**: Teams like Mumbai Indians and Chennai Super Kings invested heavily in retained players, while new teams like Lucknow Super Giants and Gujarat Titans relied on draft picks.
- **Top Spenders**: The highest costs were observed for top teams, with a peak purchase cost of 15.25 Cr for a single player by Mumbai Indians.
- **Affordable Players**: Many players were listed at low base prices, particularly bowlers, offering cost-effective options for teams focused on budget.

## Data Visualizations

The project includes the following visualizations for deeper insights:
- **Pie Chart**: Distribution of player roles in the auction (batsman, bowler, all-rounder).
- **Bar Graph**: Sold vs. unsold player count; players bought by each team.
- **Count Plot**: Team-wise distribution of players by type.
- **Annotated Bar Plot**: Total number of players retained and bought in each team, highlighting draft-pick and auction players.

## Technologies Used

- **Python**: Core language for data processing and analysis.
- **Pandas & NumPy**: Data manipulation and preprocessing.
- **Matplotlib & Seaborn**: Visualizations for data trends and distribution.

## Skills Applied
- Data Cleaning & Preprocessing
- Exploratory Data Analysis (EDA)
- Data Visualization
- Team and Cost Trend Analysis

## Conclusion

This project provided valuable insights into the IPL auction dynamics, highlighting team-specific acquisition trends, cost distribution, and the impact of retention strategies on player acquisition. This project demonstrates my ability to perform data-driven analysis, manipulate and visualize large datasets, and extract actionable insights that can assist decision-making in sports analytics.
