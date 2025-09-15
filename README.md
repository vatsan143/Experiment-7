# Experiment-7
## Write a python program for sorting and inspect for failures. 
## Algorithm:
Start the program.
2. Get the number of elements from user
3. Get the elements to be sorted
4. Traverse the array and sort the elements one by one
5. Print the sorted array
6. Stop the program. 
# Program:
```
n = int(input("Enter the number of elements: "))  
arr = []  

try:  
    for i in range(n):  
        a = float(input("Enter the element: "))  
        arr.append(a)  

    # Bubble sort (corrected)
    for i in range(n):  
        for j in range(n - i - 1):  
            if arr[j] > arr[j + 1]:  # Compare adjacent elements  
                temp = arr[j]  
                arr[j] = arr[j + 1]  
                arr[j + 1] = temp  

    print("The array after sorting: ", end="")  
    for i in range(n):  
        print(arr[i], end=" ")  

except ValueError:  
    print("Enter a valid number")
```
# Output
<img width="733" height="62" alt="image" src="https://github.com/user-attachments/assets/10833f07-b34f-4626-9b57-5f78d364d69e" />

# Result
Thus, a program to check sorting has been written and test cases have been written and verified successfully.
