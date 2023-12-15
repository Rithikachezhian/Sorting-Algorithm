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
```
Program to sort the elements in the list using the Selection Sort algorithm.
Developed by: RITHIKA N
RegisterNumber: 23013374
'''
def selection_sort(arr):
    n=len(arr)
    for i in range(n-1):
        index=i
        for j in range(i+1,n):
            if arr[j]<arr[index]:
                index=j
        arr[i],arr[index]=arr[index],arr[i]
    return arr
    
    
arr=eval(input())
print(selection_sort(arr))





```
ii)	#Insertion Sort
```
Program to sort the elements in the list using the Insertion Sort algorithm.
Developed by: your name: RITHIKA N
RegisterNumber: 23013374
'''
def insertion_sort(arr):
    for i in range(1,len(arr)):
        a=arr[i]
        j=i-1
        
        while j>=0 and a<arr[j]:
            arr[j+1]=arr[j]
            j-=1
        arr[j+1]=a
    return arr
    
arr=eval(input())
print(insertion_sort(arr))





```

## Output:
![Screenshot 2023-12-15 101555](https://github.com/Rithikachezhian/Sorting-Algorithm/assets/145742406/9bdb076a-d1ff-4217-a75b-92a1ed0d15bd)
![Screenshot 2023-12-15 101637](https://github.com/Rithikachezhian/Sorting-Algorithm/assets/145742406/03b50163-bfda-480d-9293-0e29d16800d0)



## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
