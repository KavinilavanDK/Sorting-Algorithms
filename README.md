## DATE:
## EX NO 8: Selection sort and Insertion sort
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

i)	Selection Sort
```
# DEVELOPED BY : KAVI NILAVAN
# REGISTER NUMBER : 212223230103
def selection_sort(nums):
    for i in range(len(nums)):
        lowest = i
        for j in range(i+1,len(nums)):
            if nums[j]<nums[lowest]:
                lowest = j
        nums[i],nums[lowest] = nums[lowest], nums[i]
    
list_of_nums = eval(input())
selection_sort(list_of_nums)
print(list_of_nums)
```
ii)	Insertion Sort

```
# DEVELOPED BY : KAVI NILAVAN
# REGISTER NUMBER : 212223230103
def insertion_sort(nums):
    for i in range(1,len(nums)):
        item = nums[i]
        j = i-1
        while j>=0 and nums[j]>item:
            nums[j+1]=nums[j]
            j -=1
        nums[j+1] = item
    
list_of_nums = eval(input())
insertion_sort(list_of_nums)
print(list_of_nums)
```

## Output:

### i)
![Screenshot 2024-10-16 151239](https://github.com/user-attachments/assets/4edef6aa-8cf2-4f6f-90aa-7de5920665f1)

### ii)
![Uploading Screenshot 2024-10-16 151254.png…]()


## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
