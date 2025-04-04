import matplotlib.pyplot as plt

plt.figure(figsize=(10, 5))
plt.plot(df['Month'], df['Sales'], marker='o', label='Sales', color='blue')
plt.plot(df['Month'], df['Profit'], marker='o', label='Profit', color='green')
plt.title('Monthly Sales and Profit')
plt.xlabel('Month')
plt.ylabel('Amount ($)')
plt.xticks(rotation=45)
plt.legend()
plt.grid()
plt.tight_layout()
plt.savefig('sales_profit_plot.png')  # Save the plot as an image
plt.show()
