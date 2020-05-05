# TeamSlayers

1)import pandas as pd
import numpy as np
import scipy as sp
import chart_studio.plotly as py
import matplotlib.pyplot as plt
import plotly.figure_factory as ff
import chart_studio as cs
import csv

2)with open('cars.csv', newline='') as f:                        
    reader = csv.reader(f, delimiter=';')
    for row in reader:
        print(row)

  with open('cereal.csv', newline='') as f:
    reader = csv.reader(f, delimiter=';')
    for row in reader:
        print(row)




3)df = pd.read_csv('cars.csv',delimiter=';', nrows=20, skiprows=[1])
df = pd.read_csv('cereal.csv',delimiter=';', nrows=25, skiprows=[1])


y = df['name'];
x = df['potass']

y = df['Weight'];
x = df['Horsepower']



4)plt.xlabel('Horsepower'); plt.ylabel('Weight')

plt.xlabel('potass'); plt.ylabel('name')

5)plt.scatter(x,y)

6)plt.bar(x,y)

7)plt.plot(x,y)



8)colors = ["#1f77b4", "#d62728", "#2ca02c", "#8c564b","#ff7f0e"]
plt.pie(y, labels=x, colors=colors, shadow=True, startangle=140)
plt.show()
