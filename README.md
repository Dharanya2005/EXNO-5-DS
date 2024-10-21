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
 ```
NAME : DHARANYA N
REG NO : 212223230044
```
```
import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt
```
## LINE PLOT:
```
marks=[13,45,63,78]
student=['ABC','QOR','EFB','TOB']
plt.plot(marks,student)
plt.xlabel('Marks')
plt.ylabel('Student name')
plt.show()
```
![image](https://github.com/user-attachments/assets/30b064f8-aac9-4b8d-bf35-17a17e9b9526)
```
students=['A','B','C','D']
attendence=[90,85,73,88]
plt.plot(attendence,students)
plt.xlabel('Attendence')
plt.ylabel('Student name')
plt.show()
```
![image](https://github.com/user-attachments/assets/6d51531c-7e4f-42ce-a431-d2e48d420530)

### SCATTER PLOT:
```
x=[10,20,30,40,50]
y=[100,200,300,400,500]
plt.scatter(x,y,label='stars',color='green',marker='*',s=30)
plt.show()
```
![image](https://github.com/user-attachments/assets/615442f6-825a-485c-b2c8-6a48b1699aee)
```
x=np.arange(0,15)
y=np.arange(0,15)
x
y
plt.scatter(x,y,c='r')
plt.xlabel('x axis')
plt.ylabel('y axis')
plt.title('Scatter plot')
plt.show()
```
![image](https://github.com/user-attachments/assets/9ac15b44-f0fd-4cd0-95c8-ccfe5c418d52)
### PIE CHART:
```
act=['eat','sleep','work','play']
slices=[3,7,8,6]
color=['r','y','g','b']
plt.pie(slices,labels=act,colors=color,startangle=90,shadow=True,explode=(0.1,0.1,0.1,0.1),radius=1.2,autopct='%1.1f%%')
plt.legend()
plt.show()
```
![image](https://github.com/user-attachments/assets/21251872-514e-4ee0-a2dc-2e06b2360825)

```
feedback=['Good','excellent','Perfect','Ok']
slices=[4,10,3,8]
color=['y','r','b','g']
plt.pie(slices,labels=feedback,colors=color,startangle=90,shadow=True,explode=(0.1,0.1,0.1,0.1),radius=1.2,autopct='%1.1f%%')
plt.legend()
plt.show()
```
![image](https://github.com/user-attachments/assets/26a807d6-123c-436a-9403-42614b089ddf)

# AREA CHART:
```
x = [1, 2, 3, 4, 5]
y1 = [10, 12, 14, 16, 18]
y2 = [5, 7, 9, 11, 13]
y3 = [2, 4, 6, 8, 10]
plt.fill_between(x, y1, color='blue')
plt.fill_between(x, y2, color='green')
plt.plot(x, y1, color='red')
plt.plot(x, y2, color='black')
plt.legend(['y1','y2'])
plt.show()
```
![Screenshot 2024-10-21 155805](https://github.com/user-attachments/assets/1b31d78e-bfcf-44dd-89e0-6a7235966be9)

# BAR CHART:
```
height = [10, 24, 36, 40, 5]
names = ['one', 'two', 'three', 'four', 'five']
c1=['red', 'green'] 
c2=['b', 'g']
plt.bar (names, height, width=0.8, color=c1)
plt.xlabel('x - axis')
plt.ylabel('y - axis')
plt.title('My bar chart!')
plt.show()
```
![Screenshot 2024-10-21 155940](https://github.com/user-attachments/assets/d60a4583-80c1-4a9e-a601-2c0108389546)

# HISTOGRAM:
```
x = [2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
plt.hist(x, bins = 10, color='blue', alpha=0.5)
plt.show()
```
![image](https://github.com/user-attachments/assets/a4bf7b10-1136-4169-ae39-a39009d56a70)
# BOX PLOT:
```
np.random.seed(0)
data=np.random.normal(loc=0, scale=1, size=100)
data
```
![image](https://github.com/user-attachments/assets/a340c576-db05-4b8c-9f59-fa8a227c99ac)

```
fig, ax= plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')
```
# Result:
Thus, all the data visualization techniques of matplotlib has been implemented.
