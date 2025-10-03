# visualization-generation-in-data-science
import matplotlib.pyplot as plt
import pandas as pd
# Sample data
departments = ['Finance', 'IT', 'HR','marketing','Legal']
incidents = [12, 25, 5, 18, 9]

# Create column chart
plt.figure(figsize=(8,5))
plt.bar(departments, incidents, color='mediumseagreen')
plt.title('Security Incidents by Department')
plt.xlabel('Department')
plt.ylabel('Number of Incidents')
plt.grid(axis='y', linestyle='--', alpha=0.7)
plt.tight_layout()
plt.savefig('column_chart.png')  # Saves the chart as an image
plt.show()
