# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

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
### Simple two lines:
```
import matplotlib.pyplot as plt
x1=[1,2,3]
y1=[1,4,1]
plt.plot(x1,y1, label="line 1", color="maroon", linewidth=2)

x2=[1,2,3]
y2=[4,1,4]
plt.plot(x2,y2, label="line 2", color="black", linewidth=2)

plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title("Two lines on same graph")
plt.legend()
```
![image](https://github.com/Kousalya22008930/EXNO-5-DS/assets/119389108/74fe7b42-0f1b-40cd-84ce-355a04d447a8)
### Customization of plots: 
```
import matplotlib.pyplot as plt
x = [1,2,3,4,5,6]
y = [2,4,1,5,2,6]
plt.plot(x, y, color='green', linestyle='dashed', linewidth = 3, marker='o', markerfacecolor='blue', markersize=12)

plt.xlim(1,8)
plt.ylim(1,8)

plt.xlabel('x - axis')
plt.ylabel('y - axis')

plt.title('Some cool customizations!')
plt.show()
```
![image](https://github.com/Kousalya22008930/EXNO-5-DS/assets/119389108/e285e6b4-a25f-4727-87b1-e1edf76ca0fa)
### Implementation using Matplotlib
```
yield_orange=[0.895, 0.91, 0.919, 0.926, 0.929, 0.931]
plt.plot(yield_orange, color='blue', linewidth=3)
```
![image](https://github.com/Kousalya22008930/EXNO-5-DS/assets/119389108/251e0b6e-5b31-44e1-9545-c35d5eccb446)
```
years= [2010, 2011, 2012, 2013, 2014, 2015]
yield_apples=[0.895, 0.91, 0.919, 0.926, 0.929, 0.931]
plt.plot(years, yield_apples, color='blue', linewidth=3)
```
![image](https://github.com/Kousalya22008930/EXNO-5-DS/assets/119389108/17f803c5-171d-4aa7-a2a5-b434966ee322)
```
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
![image](https://github.com/Kousalya22008930/EXNO-5-DS/assets/119389108/4767dc1b-c0d2-4f2a-8c0d-a941a59a8f71)
```
plt.figure(figsize=(12, 6))
plt.plot(years, oranges, marker='o')
plt.title("vield of Oranges (tons per hectare)")
```
![image](https://github.com/Kousalya22008930/EXNO-5-DS/assets/119389108/c092abd0-8589-4b58-93e3-c3fd1c8c1ed0)
```
plt.plot(years, apples, marker='o')
plt.plot(years, oranges, marker="x")
plt.xlabel('Year') 
plt.ylabel('Yield (tons per hectare)')
plt.title("Crop Yields in Kanto")
plt.legend([ 'Apples', 'Oranges'])
```
![image](https://github.com/Kousalya22008930/EXNO-5-DS/assets/119389108/e9ca6177-11fc-436b-9f13-60ba1d8926b0)
### Scatter Plot:
```
import matplotlib.pyplot as plt
x_values = [0,1,2,3,4,5]
y_values = [0,1,4,9,16,25]
plt.scatter(x_values, y_values,s=30, color="blue") 
plt.show()
```
![image](https://github.com/Kousalya22008930/EXNO-5-DS/assets/119389108/e935d8d7-1ce8-4c3a-8081-3bf464505a6e)
```
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd
x=np.arange(0,10)
y=np.arange(11,21)
```
![image](https://github.com/Kousalya22008930/EXNO-5-DS/assets/119389108/a953af38-4c67-43e9-9f0f-001cc549cb76)
```
plt.scatter(x,y,c="r")
plt.xlabel( 'X axis')
plt.ylabel('Y axis')
plt.title( 'Graph in 2D')
plt.savefig('Test.png')
```
![image](https://github.com/Kousalya22008930/EXNO-5-DS/assets/119389108/517c3d53-53f3-444e-b6d6-d533d7d8725f)

```
plt.plot(x,y, 'g*',linestyle='dashed' ,linewidth=2, markersize=12)
plt.xlabel( 'X axis') 
plt.ylabel( 'Y axis')
plt.title('2d Diagram')
```
![image](https://github.com/Kousalya22008930/EXNO-5-DS/assets/119389108/c59ca20d-d60c-4e88-9cdc-c82f2b8f5c1f)
```
x = np.arange(0, 4 * np.pi, 0.1) 
y= np.sin(x)
plt.title('sine wave form')
plt.plot(x, y)
plt.show()
```
![image](https://github.com/Kousalya22008930/EXNO-5-DS/assets/119389108/cfc15bf4-cbdd-458a-ac27-5b962dc5511b)
### Area Chart:

```
import matplotlib.pyplot as pit
import numpy as np
x=[1,2,3,4,5]
y1=[10, 12, 14, 16, 18]
y2=[5,7,9, 11, 13]
y3=[2,4,6,8,10]
pit.fill_between(x, y1, color='blue')
plt.fill_between(x, y2, color='green') 
plt.plot(x, y1, color='red')
plt.plot(x, y2, color='black')
plt.legend(['y1','y2'])
plt.show()
```
![image](https://github.com/Kousalya22008930/EXNO-5-DS/assets/119389108/7c193323-c454-44d6-93b3-e05f7830d4de)

### Bar Chart:
```
import matplotlib.pyplot as plt

height = [10, 24, 36, 40, 5]
names = ['one','two"', 'three’', 'four', 'five']

c1 =['chocolate', 'darkgreen']
c2 =['skyblue', 'blue'] 
plt.bar(names, height, width=0.8, color=c1)

plt.xlabel('x - axis')

plt.ylabel('y - axis')

plt.title('My bar chart!')

plt.show()
```
![image](https://github.com/Kousalya22008930/EXNO-5-DS/assets/119389108/8adfd246-70b4-4adc-8318-5f00a3b24db6)
```
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
![image](https://github.com/Kousalya22008930/EXNO-5-DS/assets/119389108/f0d347d6-be3d-4d99-a283-85ac7f537db9)
### Histogram
```
import matplotlib.pyplot as plt
ages=[2,5,70,40,30,45,50,45,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
range = (0, 100)
bins = 10
plt.hist(ages, bins, range, color='darkgreen' , histtype='bar', rwidth=0.8)
plt.xlabel('age') 
plt.ylabel('No.Of.People')
plt.title('My Histogram')
plt.show()
```
![image](https://github.com/Kousalya22008930/EXNO-5-DS/assets/119389108/ce3ec7b6-66a1-47e1-abfe-1242050c19bf)
### BOX PLOT:
```
import matplotlib.pyplot as plt
import numpy as np 

np.random.seed(0) 
data = np.random.normal(loc=0, scale=1, size=100)
data
```
![image](https://github.com/Kousalya22008930/EXNO-5-DS/assets/119389108/94c28826-41f9-49f7-b78a-b58c1f39901b)
```
fig, ax = plt.subplots() 
ax.boxplot(data) 
ax.set_xlabel('Data') 
ax.set_ylabel('values')
ax.set_title('Box Plot')
```
![image](https://github.com/Kousalya22008930/EXNO-5-DS/assets/119389108/cedf6a0f-4508-4b61-a93b-3190ed3b196a)
### Pie Chart
```
labels = 'Python', 'C++', 'Ruby', 'Java'
sizes = [215, 130, 245, 210]
colors = ['gold', 'yellowgreen', 'lightcoral', 'lightskyblue']
explode = (0, 0.4, 0, 0.5)

plt.pie(sizes, explode=explode, labels=labels, colors=colors, autopct='%1.1f%%', shadow=True)
plt.axis('equal')
plt.show()
```
![image](https://github.com/Kousalya22008930/EXNO-5-DS/assets/119389108/27c81078-bfb4-4e94-bf70-0d199fbe3353)
```
activities = ['eat', 'sleep', 'work', 'play']
slices =[3,7,8,6]
colors=['r', 'y', 'g', 'b']
plt.pie(slices, labels = activities, colors=colors, startangle=90, shadow = True, explode = (0, 0, 0.1, 0), radius = 1.2, autopct = '%1.1F%%')
plt.legend()
```
![image](https://github.com/Kousalya22008930/EXNO-5-DS/assets/119389108/0b6e08e0-8d0f-4db4-8d4a-66e36b0f71d7)


# Result:
Thus the program to Perform Data Visualization using matplot python library for the given datas is been implemented.
