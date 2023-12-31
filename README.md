# Selection sort and Insertion sort
## Aim:
To write a program to perform selection sort and insertion sort using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:-
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
### Selection Sort
```python
''' 
Program to sort the elements in the list using the Selection Sort algorithm.
Developed by: NATARAJ KUMARAN S
RegisterNumber: 23003973
'''
def selection_sort(nums):
    for i in range(len(nums)):
        lvi=i
        for j in range(i+1,len(nums)):
            if nums[j]<nums[lvi]:
                lvi=j
        nums[i],nums[lvi]=nums[lvi],nums[i]

lon=eval(input())     
selection_sort(lon)
print(lon)
    
```
### Insertion Sort
```python
''' 
Program to sort the elements in the list using the Insertion Sort algorithm.
Developed by: NATARAJ KUMARAN s
RegisterNumber: 23003973
'''
def insertion_sort(nums):
    for i in range(1,len(nums)):
        ioi=nums[i]
        j=i-1
        while j>=0 and nums[j]>ioi:
            nums[j+1]=nums[j]
            j-=1
        nums[j+1]=ioi
        
        
list_of_nums = eval(input())
insertion_sort(list_of_nums)
print(list_of_nums)    
```

## Output:
### Selection Sort
![Screenshot 2023-12-31 145800](https://github.com/nataraj26/Sorting-Algorithm/assets/147514615/3e9927d7-21cc-4abc-b278-e306bb838cae)
### Insertion Sort
![Screenshot 2023-12-31 152402](https://github.com/nataraj26/Sorting-Algorithm/assets/147514615/bbfe7b68-84fd-475b-92a1-2826cbf90faf)

## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
