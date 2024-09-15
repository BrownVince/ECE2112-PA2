<div align="center">

# Hi! <img src="https://github.com/user-attachments/assets/d21e6cd6-76a9-4934-8910-809aa4815251" alt="Wave" width="30"/>, I'm Vince Joriz E. Supsup  
From 2ECE-D, and this is my Programming Assignment #2 in ECE2112  
Submitted: Sept. 09, 2024 

</div>

# Version History
V1.0 (09-09-24) - Initial Release and Submission of Github Link  
V2.0 (09-15-24) - Edited Documentation in the Readme File  
V2.1 (09-15-24) - Added Designs in the Readme File

# Software(s) Used
<img src="https://github.com/user-attachments/assets/32ea11b3-b4e5-4efa-a673-ce2b102ab4b5" alt="Jupyter Logo" width="80"/> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub Logo" width="100"/>

# NORMALIZATION PROBLEM
### This problem involves the normalization of a set of values in a data set, which features centering, the subtraction of values from the mean, and scaling, the division of the centered values from the standard deviation
* In the normalization problem, I first tried using random.random(), but the outputs are only in float. Therefore, I tried using other functions in order to create a random array with int values, so I used random.choice(), then set the values from 0-100 and set the size to 5x5. 
```
import numpy as np
sample = np.random.choice(100, size=(5,5))
```
* After that, I used .mean() and .std() to calculate for the mean and standard deviation respectively. Furthermore, for the computation part, I tried to split it in to two parts, the centering and scaling process.
```
mean = X.mean() 
std = X.std()
cent = (X-mean)
scale = cent/std #The variable scale is final normalized array
```
* For the last part I saved the array in a file and named it 'X_normalized.npy', then I tried to load it to check if it is successfuly saved
```
np.save('X_normalized.npy', scale)
np.load('X_normalized.npy')
```
**FINAL CODE:**
![Screenshot (9)](https://github.com/user-attachments/assets/4337d33c-83b2-468e-837d-0dea9b397975)

# DIVISIBLE BY 3 PROBLEM
### This problem checks the numbers that are divisible by 3 in the set of values in an array of positive integers
* For the next problem, I used .arange() to create an array with values ranging from 1-100 instead of .linspace(), then I squared the array since the problem asked for squares of the first 100 positive integers. 
```
import numpy as np
num = np.arange(1,101)
sqnum = num**2
```
* After that, I used the .reshape() function since it can return a value so that I can store it into a new variable since I don't want to ruin the original array. 
```
sqnum10 = sqnum.reshape(10,10)
```
* Furthermore, I used the modulo function in order to check the numbers that are divisible by 3 then store it in a new variable.
```
divby3 = sqnum10[sqnum10%3 == 0]
```
* I then saved the final array into 'div_by_3.npy' then loaded it to check if the array is successfully saved.
```
np.save('div_by_3.npy', divby3)
np.load('div_by_3.npy')
```
**FINAL CODE:**
![Screenshot (10)](https://github.com/user-attachments/assets/0c03f022-b1e7-4f0e-a365-19324c1bf81c)
