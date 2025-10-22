**Cars Dataset Analysis – Python (Pandas & Matplotlib)**
**Overview**

This project explores a Cars Dataset using Pandas for data manipulation and Matplotlib for visualization. The goal was to analyze car specifications such as price, performance, fuel efficiency, and type to extract meaningful business insights and visualize trends effectively.

**Key Steps Performed**

**Data Loading & Exploration:**

Loaded the dataset using Pandas

Used .head(), .tail(), .shape, and .size to understand structure

Checked column types with .info() and identified missing values

**Data Cleaning:**

Removed duplicate entries using .duplicated() and .drop_duplicates()

Cleaned MSRP and Invoice columns by removing $ and ,

Handled inconsistent or missing numeric values

**Data Analysis:**

Counted unique categories with .nunique() and .unique()

Used .groupby() to analyze trends by Type and Origin

Aggregated data to compute average prices, mileage, and performance

**Visualizations Created (Matplotlib)**

**Line Chart:**
Average Horsepower by Engine Size

plt.plot(line_data['EngineSize'], line_data['Horsepower'])


**Bar Chart:**
Average MSRP by Car Type

plt.bar(data.groupby('Type')['MSRP'].mean().index, data.groupby('Type')['MSRP'].mean())


**Pie Chart:**
Car Distribution by Origin

plt.pie(data['Origin'].value_counts(), labels=data['Origin'].unique())


**Scatter Plot:**
Horsepower vs. MPG (City)

plt.scatter(data['Horsepower'], data['MPG_City'])

**Key Insights**

Higher engine sizes correlate with higher horsepower.

Luxury and sports car types have higher average MSRP.

The majority of vehicles originate from a few dominant regions.

Efficient cars show an inverse relationship between horsepower and city MPG.

**Skills & Tools Used**

Pandas: Data cleaning, transformation, aggregation

Matplotlib: Data visualization (line, bar, pie, scatter)

Python: Data analysis and exploratory scripting
