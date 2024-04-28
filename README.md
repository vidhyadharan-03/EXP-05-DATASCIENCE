# EXP-05-DATASCIENCE
# Aim:
  To Perform Data Visualization using matplot python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:
### Simple two lines
```python
import matplotlib.pyplot as plt
x1=[1,2,3]
y1=[1,4,1]
plt.plot(x1,y1, label="line 1", color="maroon", linewidth=2)

x2=[1,2,3]
y2=[4,1,4]
plt.plot(x2,y2, label="line 2", color="black", linewidth=2)

plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title("Two lines on the same graph")
plt.legend()
```
![image](https://github.com/varshasharon/EXNO-5-DS/assets/98278161/002adf5a-97bc-437d-8d6a-1b964d1c6d46)

### Customization of plots
```python
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]
plt.plot(x,y,color='grey', linestyle='dashed', linewidth=3, marker='o', markerfacecolor='maroon',markersize=10)

plt.ylim(1,8)
plt.xlim(1,8)

plt.xlabel('x-axis')
plt.ylabel('y-axis')

plt.title("Customization of Plots")
```
![image](https://github.com/varshasharon/EXNO-5-DS/assets/98278161/eb018fda-6e86-4df0-a3a8-ba67d5ddf632)

### Implementation using Matplotlib
```python
yield_orange=[0.895, 0.91, 0.919, 0.926, 0.929, 0.931]
plt.plot(yield_orange, color='sienna', linewidth=3)
```
![image](https://github.com/varshasharon/EXNO-5-DS/assets/98278161/0e5e95df-fbc5-4932-ac5a-9d0473167431)

```python
years= [2010, 2011, 2012, 2013, 2014, 2015]
yield_apples=[0.895, 0.91, 0.919, 0.926, 0.929, 0.931]
plt.plot(years, yield_apples, color='chocolate', linewidth=3)
```
![image](https://github.com/varshasharon/EXNO-5-DS/assets/98278161/97d24b81-513d-4e88-8db5-7b3ba45ad3be)

```python
years = range(2000, 2012) 
apples = [0.895, 0.91, 0.919, 0.926, 0.929, 0.931, 0.934, 0.936, 0.937, 0.9375, 0.9372, 0.939]
oranges = [0.962, 0.941, 0.930, 0.923, 0.918, 0.908, 0.907, 0.904, 0.901, 0.898, 0.9, 0.896, ] 
 
plt.xlabel('Year')
plt.ylabel('Yield (tons per hectare)'); 


plt.plot(years, apples)
plt.plot(years, oranges)

plt.xlabel( 'Year')
plt.ylabel('Yield (tons per hectare)')
plt.title("Crop Yields in Kanto")
plt.legend(['Apples', 'Oranges'])
```
![image](https://github.com/varshasharon/EXNO-5-DS/assets/98278161/40620a05-10f9-46c4-b1ef-fec22a2f44ce)

```python
plt.figure(figsize=(12, 6))
plt.plot(years, oranges, marker='o')
plt.title("vield of Oranges (tons per hectare)") 
```
![image](https://github.com/varshasharon/EXNO-5-DS/assets/98278161/7240f811-daee-4a9a-acb0-b7921fcecc67)

```python
plt.plot(years, apples, marker='o')
plt.plot(years, oranges, marker="x")
plt.xlabel('Year') 
plt.ylabel('Yield (tons per hectare)')
plt.title("Crop Yields in Kanto")
plt.legend([ 'Apples', 'Oranges']) 
```
![image](https://github.com/varshasharon/EXNO-5-DS/assets/98278161/1c1c071b-b001-407c-8f1f-d3a673443d18)

### Scatter Plot
```python
import matplotlib.pyplot as plt
x_values = [0,1,2,3,4,5]
y_values = [0,1,4,9,16,25]
plt.scatter(x_values, y_values,s=30, color="blue") 
plt.show() 
```
![image](https://github.com/varshasharon/EXNO-5-DS/assets/98278161/376aa83f-e208-4672-994f-7101d575fa80)

```python
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd
x=np.arange(0,10)
y=np.arange(11,21)
```
![image](https://github.com/varshasharon/EXNO-5-DS/assets/98278161/3c1770fb-7d88-4ed7-a150-55be14618969)

![image](https://github.com/varshasharon/EXNO-5-DS/assets/98278161/bef711a9-ddd6-49ff-bb17-26f3d080a123)

```python
plt.scatter(x,y,c="r")
plt.xlabel( 'X axis')
plt.ylabel('Y axis')
plt.title( 'Graph in 2D')
plt.savefig('Test.png')
```
![image](https://github.com/varshasharon/EXNO-5-DS/assets/98278161/d582fdcc-f2f3-4503-bec8-81d05dfa8581)

![image](https://github.com/varshasharon/EXNO-5-DS/assets/98278161/7a01f98b-1e1f-47a5-a04e-c0720e308590)

```python
plt.plot(x,y, 'g*',linestyle='dashed' ,linewidth=2, markersize=12)
plt.xlabel( 'X axis') 
plt.ylabel( 'Y axis')
plt.title('2d Diagram') 
```
![image](https://github.com/varshasharon/EXNO-5-DS/assets/98278161/c778f1eb-9e6d-4d85-aa87-dc115db5e1bb)

![image](https://github.com/varshasharon/EXNO-5-DS/assets/98278161/1d0a16e4-1402-4725-9696-a66465327143)

```python
x = np.arange(0, 4 * np.pi, 0.1) 
y= np.sin(x)
plt.title('sine wave form')
plt.plot(x, y)
plt.show() 
```
![image](https://github.com/varshasharon/EXNO-5-DS/assets/98278161/ecd74a1b-8eeb-44b4-a592-ea20184e73c1)

### Area Chart
```python
import matplotlib.pyplot as pit
import numpy as np
x=[1,2,3,4,5]
y1=[10, 12, 14, 16, 18]
y2=[5,7,9, 11, 13]
y3=[2,4,6,8,10]
pit.fill_between(x, y1, color='maroon')
plt.fill_between(x, y2, color='orange') 
plt.plot(x, y1, color='red')
plt.plot(x, y2, color='black')
plt.legend(['y1','y2'])
plt.show() 
```
![image](https://github.com/varshasharon/EXNO-5-DS/assets/98278161/2237fffd-023e-465f-a62c-2553fbf81f5c)

### Bar Chart
```python
import matplotlib.pyplot as plt

height = [10, 24, 36, 40, 5]
names = ['one','two"', 'three’', 'four', 'five']

c1 =['chocolate', 'darkgreen']
c2 =['skyblue', 'blue'] 
plt.bar(names, height, width=0.8, color=c1)

plt.xlabel('x - axis')

plt.ylabel('y - axis')

plt.title('Bar Chart')

plt.show() 
```
![image](https://github.com/varshasharon/EXNO-5-DS/assets/98278161/60c652ad-619b-4720-a076-0ffe932e29b9)

```python
x = [2,8,10]
y = [11,16,9]
x2 = [3,9,11]
y2 = [6,15,7] 
plt.bar(x, y,color='chocolate')
plt.bar(x2, y2, color = 'darkgreen')
plt.title('Bar graph')
plt.ylabel('Y axis')
plt.xlabel('X axis')
plt.show() 
```
![image](https://github.com/varshasharon/EXNO-5-DS/assets/98278161/b23a89ae-b968-4487-bde3-8360572970da)

### Histogram
```python
import matplotlib.pyplot as plt

ages=[2,5,70,40,30,45,50,45,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
range = (0, 100)
bins = 10

plt.hist(ages, bins, range, color='darkgreen' , histtype='bar', rwidth=0.8)

plt.xlabel('age') 

plt.ylabel('No. of people')

plt.title('My histogram')

plt.show() 
```
![image](https://github.com/varshasharon/EXNO-5-DS/assets/98278161/6570d720-045d-40e7-b287-6f7722a4d5ed)

### Box Plot
```python
import matplotlib.pyplot as plt
import numpy as np 

np.random.seed(0) 
data = np.random.normal(loc=0, scale=1, size=100)
data 
```
![image](https://github.com/varshasharon/EXNO-5-DS/assets/98278161/55eb17fa-98e9-44c6-8e6c-e42b4fd30ff2)

```python
fig, ax = plt.subplots() 
ax.boxplot(data) 
ax.set_xlabel('Data') 
ax.set_ylabel('Values')
ax.set_title('Box Plot') 
```
![image](https://github.com/varshasharon/EXNO-5-DS/assets/98278161/a7a684a7-4b2b-4b39-b8b0-e44132ec9b09)

### Pie Chart
```python
labels = 'Python', 'C++', 'Ruby', 'Java'
sizes = [215, 130, 245, 210]
colors = ['gold', 'yellowgreen', 'lightcoral', 'lightskyblue']
explode = (0, 0.4, 0, 0.5)

plt.pie(sizes, explode=explode, labels=labels, colors=colors, autopct='%1.1f%%', shadow=True)
plt.axis('equal')
plt.show() 
```
![image](https://github.com/varshasharon/EXNO-5-DS/assets/98278161/bcb6b879-9c44-4cde-b6c6-d235b9b38d99)

```python
activities = ['eat', 'sleep', 'work', 'play']

slices =[3,7,8,6]

colors=['r', 'y', 'g', 'b']

plt.pie(slices, labels = activities, colors=colors, startangle=90, shadow = True, explode = (0, 0, 0.1, 0), radius = 1.2, autopct = '%1.1F%%')

plt.legend()
```
![image](https://github.com/varshasharon/EXNO-5-DS/assets/98278161/b3174e4d-8d2e-4e52-aab0-075bb07c8ac2)

# Result:
Thus, all the data visualization techniques of matplotlib has been implemented.
