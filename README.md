# Selection sort and Insertion sort
## Aim:
To write a program to perform selection sort and insertion sort using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Selection Sort Algorithm:
1.	Set the first unsorted element as the minimum
2.	For each of the unsorted elements, check if the element < current minimum.
3.	If yes, set the element as the new minimum.
4.	Swap minimum with first unsorted position.
5.	Repeat the steps 2 and 3 for all the elements in the array.
## Insertion Sort Algorithm:
1.	Set the first element as sorted element j.
2.	For each unsorted element X, check if current sorted element j >X.
3.	If yes, move sorted element to the right by 1.
4.	Break the loop and insert X.
5.	Repeat the steps 2 to 4 for sorting all the elements in the array.
## Program:
i)	#Selection Sort
 # Program to  Sort the element in the list using the Selection Sort algorithm.
 # Developed by: SANJAI S
 # Register Number:23013614
```
## Program to  Sort the element in the list using the Selection Sort algorithm.
 # Developed by: SANJAI S
 # Register Number:23013614

def selection_sort(nums):
    for i in range(len(nums)):
        lowest_value_index = i
        for j in range(i+1,len(nums)):
            if  nums[j] < nums[lowest_value_index]:
                lowest_value_index = j
        nums[i],  nums[lowest_value_index] = nums[lowest_value_index], nums[i]        
        

list_of_nums = eval(input())
selection_sort(list_of_nums)
print(list_of_nums)
```
ii)	#Insertion Sort
 # Program to  Sort the element in the list using the Insertion Sort algorithm.
 # Developed by: SANJAI S
 # Register Number:23013614
```
def insertion_sort(arr):
    n=len(arr)
    if n<=1:
        return
    for i in range(1,n):
        key=arr[i]
        j=i-1
        while j>=0 and key<arr[j]:
            arr[j+1]=arr[j]
            j-=1
        arr[j+1]=key
    
    
    
arr = eval(input())
insertion_sort(arr)
print(arr)
```

## Output:
![Screenshot 2023-12-31 140815](https://github.com/Sanjaichitra/Sorting-Algorithm/assets/144870518/4ffe7515-1e4d-4b28-941b-cd73bca632bd)
![Screenshot 2023-12-31 141020](https://github.com/Sanjaichitra/Sorting-Algorithm/assets/144870518/dc573f7f-1b34-4377-a0b0-5c58b38c320f)


## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
