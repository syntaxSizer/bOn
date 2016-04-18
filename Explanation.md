# Big O notation


What is the big O notation and why its called big O notation anyway ?

Big O notation: also called Landau's symbol, is a
symbolism used in complexity theory, computer science, and mathematics to describe the
asymptotic behavior of functions. Basically, it tells you how fast a function grows or
declines.

Landau's symbol comes from the name of the German number theoretician Edmund
Landau who invented the notation. The letter O is used because the rate of growth of a
function is also called its order





## Notations                   Name

### O(1)                       constant
### O(log(n))                  logarithmic
### O((log(n))^c)              polylogarithmic
### O(2^n                      explontial
### O(n)                       linear
### O(n^2)                     quadratic



## Underestanding Big O
is a way to measure  how well a computer algorithm  scales as the amount of data involved increases
and it has nothing to do with speed.



## Order of one O(1)

O(1) Execute in a constant  amount of time regardless of the amount of data

Example :
it i'll execute the in same amount of time  10 array items or 10,000 array items
in other words, the time accessing the collection is independant from the number of the collection items (constant opartion time)

this code will add new item to the array it won't matter if the array had 10 items or 10^10 items
```java
int theArray[];
int itemInArray=0;
public void addItemToArray(int newItem){
theArray[itemsInArray++]=newitem;

}
```


## Order of n  O(N)
it mean the amount of time to complete will grow up indierct proportion to the amont of data .

Example linear search:
in order to find a match for what we are searching for we will have to look in every and each item .
it will matter if we are searching in total of 10 items or 10,000 items .

```java
public void linearSearchForValue(int value){
	boolean valueInArray=false;
	String indexWithValue="";


	for(int i=0; i< arraySize; i++){
		if(theArray[i]==value){
			valueInArray = true;
			indexWithValue+=i +" ";

		}
	}

	```


## Order of n log n O(nLogn)
it combines the linear complexity and the logarithmic complexity.
a good example is the merge sort.

in the merge sort we divide the list in two again and again until we are left with a number of list items with one item in each of these lists is sorted. we then merge each list with the neighbour. werepeat this with the new composite list until we have a sorted result.



## Order of log n
the time taken increases with the size of the data set , but not proportionately. this means algorithm takes longer per item on smaller datasets rlative to larger ones.
an example is the binary search



