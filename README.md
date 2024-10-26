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

import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as pl

Line Plot:

marks=[13,45,63,78]
student=['ABC','QOR','EFB','TOB']
plt.plot(marks,student)
plt.xlabel('Marks')
plt.ylabel('Student name')
plt.show()

student=['A','B','C','D']
attendence=[90,85,73,88]
plt.plot(attendence,student)
plt.xlabel('Attendence')
plt.ylabel('Student name')
plt.show()

![Screenshot 2024-10-26 110827](https://github.com/user-attachments/assets/764fad78-3da2-4bbc-8dab-1d0910510e0d)

Scatter Plot:

x=[10,20,30,40,50]
y=[100,200,300,400,500]
plt.scatter(x,y,label='stars',color='green',marker='*',s=30)
plt.show()

x=np.arange(0,15)
y=np.arange(0,15)
x
y
plt.scatter(x,y,c='r')
plt.xlabel('X axis')
plt.ylabel('y axis')
plt.title('Scatter plot')
plt.show()

![Screenshot 2024-10-26 110905](https://github.com/user-attachments/assets/e92e2378-dd79-42c7-a447-acbdaca2f5fd)

Pie Chart:

act=['eat','sleep','work','play']
slices=[3,7,8,6]
color=['r','y','g','b']
plt.pie(slices,labels=act,colors=color,startangle=90,shadow=True,explode=(0.1,0.1,0.1,0.1),radius=1.2,autopct='%1.1f%%')
plt.legend()
plt.show()

feedback=['Good','excellent','Perfect','Ok']
slices=[4,10,3,8]
color=['y','r','b','g']
plt.pie(slices,labels=feedback,colors=color,startangle=90,shadow=True,explode=(0.1,0.1,0.1,0.1),radius=1.2,autopct='%1.1f%%')
plt.legend()
plt.show()

![Screenshot 2024-10-26 110936](https://github.com/user-attachments/assets/2c4a55e9-0eb3-4d6c-9cb2-cab4e4bc2e48)

Area Chart:

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

![Screenshot 2024-10-26 111020](https://github.com/user-attachments/assets/4ec91191-452c-44eb-bb3f-aba4011c0399)

Bar Chart:

height = [10, 24, 36, 40, 5]
names = ['one', 'two', 'three', 'four', 'five']
c1=['red', 'green'] 
c2=['b', 'g']
plt.bar (names, height, width=0.8, color=c1)
plt.xlabel('x - axis')
plt.ylabel('y - axis')
plt.title('My bar chart!')
plt.show()

![Screenshot 2024-10-26 111048](https://github.com/user-attachments/assets/563fddc9-4bdf-4ef6-89c9-c1454b0341f9)

Histogram:

x = [2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
plt.hist(x, bins = 10, color='blue', alpha=0.5)
plt.show()

![Screenshot 2024-10-26 111117](https://github.com/user-attachments/assets/fdc54bde-0b55-43eb-8228-ce885bdd4ad1)

Box Plot:

np.random.seed(0)
data=np.random.normal(loc=0, scale=1, size=100)
data

![Screenshot 2024-10-26 111140](https://github.com/user-attachments/assets/9ba15db7-40de-4095-8fc7-ff6e5446716c)


fig, ax= plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')

![Screenshot 2024-10-26 111157](https://github.com/user-attachments/assets/63c0d8a4-1d63-493e-9d8f-757bd07ad4f0)


# Result:
Thus, all the data visualization techniques of matplotlib has been implemented
