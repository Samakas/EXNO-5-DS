# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY
## NAME: Samakash R S
## REGISTER NO.: 212223230182
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

```
#Line Graphs
import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt
x = [1, 2, 3, 4, 5]
y = [3, 6, 2, 7, 1]
plt.plot(x,y,label='line1')
plt.show()
```
![image](https://github.com/user-attachments/assets/33d9d8f1-2be5-4cc6-8515-2f14ab45bb15)


```
#Simple 2 lines
import matplotlib.pyplot as plt

x1 = [1, 2, 3]
y1 = [2, 4, 1]
plt.plot(x1, y1, label='line 1')

x2 = [1, 2, 3]
y2 = [4, 1, 3]
plt.plot(x2, y2, label='line 2')

plt.xlabel("x-axis")
plt.ylabel("y-axis")
plt.title("Two lines on same graph!")
plt.legend()
plt.show()
```
![image](https://github.com/user-attachments/assets/1a008f0f-5b52-4982-9716-ea180b744425)

```
#Customixation of plots
import matplotlib.pyplot as plt

x = [1, 2, 3, 4, 5, 6]
y = [2, 4, 1, 5, 2, 6]

plt.plot(x,y, color='red', linewidth=3, linestyle='--', marker = 'o', markerfacecolor='blue', markersize=10)
plt.ylim(1, 8)
plt.xlim(1, 8)
plt.xlabel("x-axis")
plt.ylabel("y-axis")
plt.title("Some cool customization")
plt.show()
```
![image](https://github.com/user-attachments/assets/11f7e71f-79c6-46c5-9504-768a76107d66)

```
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(yield_apples)

years=[2010,2011,2012,2013,2014,2015]
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(years,yield_apples)
```
![image](https://github.com/user-attachments/assets/a3a077c7-4423-4647-b59c-ea6af9888a88)
![image](https://github.com/user-attachments/assets/20fc32bf-43ac-4d7b-a053-97dcaf384430)
```
years=range(2000,2012)
apples=[0.895,0.91,0.919,0.926,0.929,0.931,0.934,0.936,0.937,0.9375,0.9372,0.939]
oranges=[0.926,0.941,0.930,0.923,0.918,0.908,0.907,0.904,0.901,0.898,0.9,0.896, ]
plt.plot(years, apples)
plt.plot(years, oranges)
plt.xlabel('Year')
plt.ylabel('Yield (tons per hectare)')
plt.title('Crop Yields in Kanto')
plt.legend(['Apples','Oranges']);



plt.figure(figsize=(12,6))
plt.plot(years,oranges,marker='o')
plt.title("Yield of Oranges (tons per hectare)");

```
![image](https://github.com/user-attachments/assets/9b9324a7-ef8e-4cf2-a317-4cf5c45a0ecf)
![image](https://github.com/user-attachments/assets/1f69a294-948b-47ec-a37b-d5bb98987ab0)


```
#Scatter Plots

import matplotlib.pyplot as plt
import numpy as np
import pandas as pd
x=np.arange(0,10)
y=np.arange(11,21)

plt.scatter(x,y,c='r')
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.title('Graph in 2D')
plt.savefig('Test.png')
```
![image](https://github.com/user-attachments/assets/3e3ab396-e5a1-4df3-a000-7f38d889e98b)


```
#Customized Scatter Plot

y=x*x
y

plt.plot(x,y,'g*',linestyle='dashed',linewidth=2,markersize=12)
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.title('2d Diagram')
plt.legend(['y-values']);
```
![image](https://github.com/user-attachments/assets/c93cbedd-ba48-413c-964d-a6965d75390f)

![image](https://github.com/user-attachments/assets/be81b93f-b9ca-4fcf-b935-07266d4cf2b2)

```
#Sine wave form
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd

x=np.arange(0,4*np.pi,0.1)
y=np.sin(x)
plt.title("sine wave form")
plt.plot(x,y)
plt.show()

```
![image](https://github.com/user-attachments/assets/1fbe8f21-7faa-4ccb-8571-ee7bf05a361a)


```
#Area Chart

import matplotlib.pyplot as plt
import numpy as np
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='blue')
plt.fill_between(x,y2,color='green')
plt.plot(x,y1,color='red')
plt.plot(x,y2,color='black')
plt.legend(['y1','y2'])
plt.show()
```
![image](https://github.com/user-attachments/assets/5960db0b-b99b-4776-9b88-56ee5b35174d)

```
#Customized Bar Plot

import matplotlib.pyplot as plt

height = [10, 24, 36, 40, 5]
names = ['one', 'two', 'three', 'four', 'five']
c1 = ['red','green']
c2 = ['b','g']
plt.bar(names , height, color=c1)

plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('My bar chart')

plt.show()
```
![image](https://github.com/user-attachments/assets/d84e5268-c960-42e3-85d6-97d1bf3cc8bd)

```
#Bar plot for 2 features
import matplotlib.pyplot as plt

x = [2, 8, 10]
y = [11, 16, 9]
x2 = [3, 9, 11]
y2 = [6, 15, 7]

plt.bar(x,y,color="r")
plt.bar(x2,y2,color="g")
plt.title("Bar graph")
plt.ylabel('Y axis')
plt.xlabel('X axis')
plt.show()
```
![image](https://github.com/user-attachments/assets/548c0b93-c696-4734-879b-68d9b962e2ce)

```
#Histogram

import matplotlib.pyplot as plt

ages = [2,5,70,40,30,45,50,45,43,40,44,60,7,13,57,18,90,77,32,21,20,401]
range=(0,100)
bins=10

plt.hist(ages,bins,range,color="blue",histtype='bar',rwidth=0.8)
plt.xlabel('age')
plt.ylabel('No. of people')
plt.title('My histogram')
plt.show()
```
![image](https://github.com/user-attachments/assets/b9c5c6e3-e464-4469-bcb6-8c0b5b3dd38a)

```
import matplotlib.pyplot as plt
import numpy as np

np.random.seed(0)
data = np.random.normal(loc=0, scale=1,size=100)
data
```
![image](https://github.com/user-attachments/assets/8253da01-3b75-46e3-98da-4595203e0627)

```
fig, ax = plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')
```
![image](https://github.com/user-attachments/assets/5ed49625-2537-4702-b62d-714906f51e58)

```
#pie-chart
labels='Python','C++','Ruby','Java'
sizes=[215,130,245,210]
colors=['gold','yellowgreen','lightcoral','lightskyblue']
explode=(0,0.4,0,0.5)
plt.pie(sizes,explode=explode,labels=labels,colors=colors,autopct='%1.1f%%',shadow=True)
plt.axis('equal')
plt.show()
```
![image](https://github.com/user-attachments/assets/4773e401-0bb5-4da5-a463-b16cbf9d3e5d)

```
#Pie Chart

import matplotlib.pyplot as plt

activities = ['eat', 'sleep', 'work', 'play']
#Pie Chart

import matplotlib.pyplot as plt

activities = ['eat', 'sleep', 'work', 'play']
slices = [3, 7, 8, 6]
colors = ['r', 'y', 'g', 'b']
plt.pie(slices, labels = activities, colors=colors, startangle=90, shadow = True, explode = (0, 0, 0.1, 0), radius = 1.2, autopct = '%1.1f%%')
plt.legend()
plt.show()
```
![image](https://github.com/user-attachments/assets/1379f23f-7773-48b2-becc-797078b7a8b1)

# Result:
   Thus the data visualization using matplot python library for the given datas are performed.
