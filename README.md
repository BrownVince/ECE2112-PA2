# ECE2112-PA2
Supsup, Vince Joriz E.  
2ECE-D  
Sept. 09, 2024  
# NORMALIZATION PROBLEM
In the normalization problem, I first tried using random.random(), but the outputs are only in float. Therefore, I tried using other functions in order to create a random array with int values, so I used random.choice(), then set the values from 0-100 and set the size to 5x5. After that, I used .mean() and .std() to calculate for the mean and standard deviation respectively. Furthermore, for the computation part, I tried to split it in to two parts, the centering and scaling process then saved it into 'X_normalized.npy', then I tried to load it to check if it is actually saved.
![Screenshot (9)](https://github.com/user-attachments/assets/4337d33c-83b2-468e-837d-0dea9b397975)
# DIVISIBLE BY 3 PROBLEM
For the next problem, I used .arange() to create an array with values ranging from 1-100 instead of .linspace(), then I squared the array since the problem asked for squares of the first 100 positive integers. After that, I used the .reshape() function since it can return a value so that I can store it into a new variable since I don't want to ruin the original array. Furthermore, I used the modulo function in order to check the numbers that are divisible by 3 then store it in a new variable, then I saved the final array into 'div_by_3.npy' then loaded it to check if the array is successfully saved.
