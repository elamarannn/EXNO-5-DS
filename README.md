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
import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt

x = [1, 2, 3, 4, 5]
y = [3, 6, 2, 7, 1]

plt.plot(x,y,label = 'line1')
```
![download](https://github.com/user-attachments/assets/cee9e69a-1c3b-48f9-ade2-65bde2af837f)
```
x1 = [1,2,3]
y1 = [2,4,1]
x2 = [1,2,3]
y2 = [4,1,3]

plt.plot(x1,y1,label='line1')
plt.plot(x2,y2,label='line2')
plt.xlabel('x axis')
plt.ylabel('y axis')
plt.title('Two lines on same graph!')
plt.legend()
plt.show()
```
![download](https://github.com/user-attachments/assets/de7e15db-1cb5-4731-a64d-efa73a9ec91f)
```
import matplotlib.pyplot as plt
x = [1,2,3,4,5,6]
y = [2,4,1,5,2,6]
plt.plot(x,y,color ='green', linestyle='dashed', linewidth=3,marker='o',markerfacecolor='blue',markersize=12)
plt.xlabel('x axis')
plt.ylabel('y axis')
plt.title('Custom')
plt.show()
```
![download](https://github.com/user-attachments/assets/d31c7c82-9df5-4d1e-a546-31b745365015)
```
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(yield_apples)
```
![download](https://github.com/user-attachments/assets/dcf495b7-adaa-4940-aab7-14231938f66c)
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
```
![download](https://github.com/user-attachments/assets/1a1569b4-b9dd-4f43-b693-e3896e5b3794)
```
plt.figure(figsize=(12,6))
plt.plot(years,oranges,marker='o')
plt.title("Yield of Oranges (tons per hectare)");
```
![download](https://github.com/user-attachments/assets/4385307a-251a-4db3-81d2-a535a7be4fa2)
```
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd
x=np.arange(0,10)
y=np.arange(11,21)
x
```
![image](https://github.com/user-attachments/assets/946624cf-74fd-4a0f-97cc-a39418c22203)
```
y
```
![image](https://github.com/user-attachments/assets/4a63270b-8324-4242-a63d-d8871c6b65fd)
```
plt.scatter(x,y,c='r')
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.title('Graph in 2D')
plt.savefig('Test.png')
```
![download](https://github.com/user-attachments/assets/a3f0198f-fc47-4ebf-9cd5-d25ed9ce9789)
```
y=x*x
y
```
![image](https://github.com/user-attachments/assets/afed580d-ad49-4d31-a9ad-81ac8dc7079d)
```
plt.plot(x,y,'g*',linestyle='dashed',linewidth=2,markersize=12)
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.title('2d Diagram')
plt.legend(['y-values']);
```
![download](https://github.com/user-attachments/assets/e1d6df7d-265d-4892-8479-73a72f58b041)
```
x=np.arange(0,4*np.pi,0.1)
y=np.sin(x)
plt.title("sine wave form")
plt.plot(x,y)
plt.show()
```
![download](https://github.com/user-attachments/assets/9a752c25-afb4-41a3-a366-ab94afa6646c)
```
import matplotlib.pyplot as plt
import numpy as np
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='blue')
plt.fill_between(x,y2,color='green')
```
![download](https://github.com/user-attachments/assets/da8e2f8f-9dcb-44e7-a63c-bc9b368a4872)
```
import matplotlib.pyplot as plt
import numpy as np
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y2,color='green')
plt.plot(x,y1,color='red')
plt.plot(x,y2,color='black')
plt.legend(['y1','y2'])
plt.show()
```
![download](https://github.com/user-attachments/assets/2489ef2a-524f-44df-929e-53b8e6d39ff4)
```
import matplotlib.pyplot as plt
height=[10,24,36,40,5]
names=['one','two','three','four','five']
c1=['red','green']
c2=['b','g']
plt.bar(names,height,width=0.8,color=c1)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('My bar chart!')
plt.show()
```
![download](https://github.com/user-attachments/assets/3f82ddd5-b52d-44aa-8f70-4da65b41ad0e)
```
x=[2,8,10]
y=[11,16,9]
x2=[3,9,11]
y2=[6,15,7]
plt.bar(x,y,color='r')
plt.bar(x2,y2,color='g')
plt.title('Bar graph')
plt.ylabel('Y axis')
plt.xlabel('X axis')
plt.show()
```
![download](https://github.com/user-attachments/assets/06d3f986-e420-438c-94b0-0bc4331b4cd0)
```
import matplotlib.pyplot as plt
ages=[2,5,70,40,30,45,50,45,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
range=(0,100)
bins=10
plt.hist(ages,bins,range,color='green',histtype='bar',rwidth=0.8)
plt.xlabel('age')
plt.ylabel('No. of people')
plt.title('My histogram')
plt.show()
```
![download](https://github.com/user-attachments/assets/759900a4-0743-45b7-98de-ab49f0311324)
```
import matplotlib.pyplot as plt
import numpy as np
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data
```
![image](https://github.com/user-attachments/assets/efd61487-ad3d-4ad0-bf73-961eaf8c4611)
```
fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')
```
![download](https://github.com/user-attachments/assets/a7cb3a4a-8fc9-4ef4-a88d-882aa7d72426)
```
labels ='Python', 'C++', 'Ruby', 'Java'
sizes=[215,130,245,210]
colors=['gold', 'yellowgreen', 'lightcoral', 'lightskyblue']
explode=(0,0.4,0,0.5)
plt.pie(sizes, explode=explode, labels=labels, colors=colors, autopct='%1.1f%%', shadow=True)
plt.axis('equal')
plt.show()
```
![download](https://github.com/user-attachments/assets/bca9f7f4-9266-46f1-8e4c-40e6d5675ab2)
```
activities=['eat', 'sleep', 'work', 'play']
slices=[3,7,8,6]
colors=['r','y','g', 'b']
plt.pie(slices, labels=activities, colors=colors, startangle=90, shadow=True, explode=(0,0,0,1), radius=1.2, autopct='%1.1f%%') 
plt.legend()
```
![download](https://github.com/user-attachments/assets/0e7a0061-b73e-4abd-ba8e-3ce09515aa48)

# Result:
Thus Data Visualization using matplot python library for the given datas is performed

