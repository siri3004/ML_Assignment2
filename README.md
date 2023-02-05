# ML_Assignment2
#Q1
The right pascal triangle pattern can be clearly seen that it is made up of an upper triangle and a lower triangle. 
So, you can run 2 different for loops one which creates the upper triangle and another which creates the lower triangle. 
Also, the print("* ", end='') function prints only star accompanied by a space.

python code to display the following star pattern using the for loop
num_rows = 5
for i in range (0, num_rows):
    for j in range(0, i + 1):
        print("* ", end='')
    print("\r")
for i in range (num_rows, 0, -1):
    for j in range(0, i -1):
        print("* ", end='')
    print("\r")
