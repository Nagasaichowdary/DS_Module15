# Ex14 Heap Tree
## DATE:
## AIM:
To write a C function to delete an element in a Heap Tree.

## Algorithm
1.Start
2.Find the index of the element num in the array.
3.Swap the element to be deleted with the last element in the array.
4.Decrease the array size (size) by 1.
5.Start heapifying from the last non-leaf node (index size/2 - 1).
6.Call heapify() to restore the heap property for each node.
7.End    

## Program:
```
/*
Program to delete an element in a Heap Tree
Developed by:   P . ADITYA NAGA SAI
RegisterNumber:  212223110036
*/

voiddeleteRoot(int array[], int num)
{
int i; for(i=0;i<size;i++)
{
if(num==array[i])
{
break;
}
}
swap(&array[i],&array[size-1]); size-=1;
for(i=size/2-1;i>=0;i--)
{
heapify(array,size,i);
}
}

```

## Output:
![image](https://github.com/user-attachments/assets/69bedb98-da1e-40e9-8311-4b4abd22b4d9)



## Result:
Thus, the function to delete an element in a Heap Tree is implemented successfully.
