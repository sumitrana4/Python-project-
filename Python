import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

# Load CSV file
data = pd.read_csv("students.csv")

# Display dataset
print(data.head())

# Dataset information
print(data.info())

# Statistical summary
print(data.describe())

# Calculate average
average_math = data["Math"].mean()
print("Average Math Marks:", average_math)

# Bar Chart
plt.bar(data["Name"], data["Math"])
plt.title("Math Scores")
plt.xlabel("Students")
plt.ylabel("Marks")
plt.show()

# Scatter Plot
plt.scatter(data["Math"], data["Science"])
plt.title("Math vs Science")
plt.xlabel("Math")
plt.ylabel("Science")
plt.show()

# Heatmap
correlation = data.corr(numeric_only=True)

sns.heatmap(correlation, annot=True, cmap="coolwarm")
plt.title("Correlation Heatmap")
plt.show()
