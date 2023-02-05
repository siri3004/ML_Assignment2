# ML_Assignment2
#Q1 python code to display the following star pattern using the for loop

---> The right pascal triangle pattern can be clearly seen that it is made up of an upper triangle and a lower triangle. 

So, you can run 2 different for loops one which creates the upper triangle and another which creates the lower triangle. 

Also, the print("* ", end='') function prints only star accompanied by a space.


    num_rows = 5
    for i in range (0, num_rows):
        for j in range(0, i + 1):
            print("* ", end='')      
        print("\r") 
        
    for i in range (num_rows, 0, -1):
        for j in range(0, i -1):    
            print("* ", end='')       
        print("\r")  


#Q2 Use looping to output the elements from a provided list present at odd indexes.

my_list = [10, 20, 30, 40, 50, 60, 70, 80, 90, 100]

---> A list is defined and is displayed on the console. 

The list is iterated over beginning from the second index element, and the step size is mentioned as 2 in the range method. 

Those elements that are in odd positions are displayed on the console.


    my_list = [10, 20, 30, 40, 50, 60, 70, 80, 90, 100]
    print("The list is :")
    print(my_list)
    print("The elements in odd positions are : ")
    for i in range(1, len(my_list), 2):
        print(my_list[i])
        

#Q3 Write a code that appends the type of elements from a given list.

Input

 x = [23, ‘Python’, 23.98]
 
 Expected output
 
 [23, 'Python', 23.98]
 
 [<class 'int'>, <class 'str'>, <class 'float'>]
 
 ---> As per the given input, 
 by using append() function returns an element to insert at the end of each Element in the set of matched elements. 

 
    x = [23, 'Python', 23.98]
    type_list = []
    for item in x:
        type_list.append(type(item))
    print("Elements:",x)
    print("Types:", type_list)   


#Q4 Write a function that takes a list and returns a new list with unique items of the first list.

Sample List: [1,2,3,3,3,3,4,5]

Unique List: [1, 2, 3, 4, 5]

---> In a given input, duplicate values are not listed and append () function takes a single item as an input parameter and adds it to the end of the given list.

    def unique_list(l):
    x = []
    for a in l:
        if a not in x:
        x.append(a)
    return x

    print(unique_list([1,2,3,3,3,3,4,5]))
    

#Q5 Write a function that accepts a string and calculate the number of upper-case letters and lower-case
letters.

Input String: 'The quick Brow Fox'

Expected Output:

No. of Upper-case characters: 3

No. of Lower-case Characters: 12

---> In given string, count the number of lower-case and upper-case letters, defined a function. 

Initialize two variables. To count each letter in the string we need to iterate over each character in the string by using for loop. 

To check the letter case increment and add it to for loop and print the values at the end of the function.


    def up_low(string):
      uppers = 0
      lowers = 0
      for char in string:
        if char.islower():
          lowers += 1
        elif char.isupper():
          uppers +=1
        else: #I added an extra case for the rest of the chars that aren't lower non upper
          pass
      return(uppers, lowers)

    string ='The quick Brow Fox'
    uppers, lowers = up_low(string)
    print("No. of Upper-case characters:", uppers)
    print("No. of Lower-case characters:", lowers)



