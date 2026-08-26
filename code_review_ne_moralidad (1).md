### 

### **Annex C**

**Code Quality Assessment Worksheet**

**Section: 9 \- NEON                                                                      	Score:\_\_\_\_\_\_\_\_\_\_\_\_**  
**C\# / Name:26/Angelica Faith Moralidad,23/Sofia Princess Hijalga	Date: 08/26/24**  
   
**Instructions:**

**The problem: Search for a Number in a Sorted List**

**For example: Both algorithms could search:**   
numbers \= \[5, 12, 18, 23, 31, 47, 56, 68, 74, 90\]  
target \= 47

| Implementation 1 | Implementation 2 |
| ----- | ----- |
| def linear\_search(numbers, target):    *for* i *in* range(len(numbers)):        *if* numbers\[i\] \== target:            *return* i    *return* \-1   | def binary\_search(numbers, target):    low \= 0    high \= len(numbers) \- 1     *while* low \<= high:        middle \= (low \+ high) // 2         *if* numbers\[middle\] \== target:            *return* middle        *elif* numbers\[middle\] \< target:            low \= middle \+ 1        *else*:            high \= middle \- 1     *return* \-1   |

## 

## 

## 

## 

## **Questions with Checklists**

### **1\. Efficiency**

Which algorithm is faster when the list of numbers is very large? Why?

Algorithm 2 is faster because it implements binary search, which breaks down the search area of large numbers by calculating the midrange,

**Checklist to guide your answer:**

| Implementation 1 | Implementation 2 |
| ----- | ----- |
| ~~How many elements might the algorithm need to check? Does the algorithm reduce the search area as it runs? Does the algorithm still work efficiently with a very large list?~~ | ~~How many elements might the algorithm need to check? Does the algorithm reduce the search area as it runs? Does the algorithm still work efficiently with a very large list?~~ |

**2\. Readability**

Which algorithm is easier to understand at first glance? What makes it clearer?

To me and my partner, Implementation 2 is the more readable algorithm. Mainly because it uses the familiar if, else if and while loop codes and has simple and direct names for the variables.

**Checklist to guide your answer:**

| Implementation 1 | Implementation 2 |
| ----- | ----- |
| ~~How meaningful are the variable names? How simple is the logic? How concise is the code? How easy is it to follow the search process?~~ | ~~How meaningful are the variable names? How simple is the logic? How concise is the code? How easy is it to follow the search process?~~ |

### 

### **3\. Maintainability**

If you had to modify the program, such as changing what happens when the target is found, which algorithm would be easier to update? Why?

Implementation 1 is easier to modify because when we need to update it, we only need to change one variable or can add the change later in the code. Meanwhile, to modify Implementation 2, it is needed to change more variables than Implementation 1\. 

**Checklist to guide your answer:**

| Implementation 1 | Implementation 2 |
| ----- | ----- |
| ~~Is the structure straightforward? Would adding new steps break the code easily? Is there less chance of errors when updating?~~ | ~~Is the structure straightforward? Would adding new steps break the code easily? Is there less chance of errors when updating?~~ |

### 

### **4\. Testability**

Which algorithm is easier to test with different inputs? Why?

Implementation 1 is easier because it doesn’t need to be sorted unlike Implementation 2, which even though it’s direct, it takes a process to sort out the variables first before the process even starts.

**Checklist to guide your answer:**

| Implementation 1 | Implementation 2 |
| ----- | ----- |
| ~~Can you test with small lists easily? Does the algorithm have fewer conditions to check? Is the output predictable and clear?~~ | ~~Can you test with small lists easily? Does the algorithm have fewer conditions to check? Is the output predictable and clear?~~ |

### **5\. Reliability and Input Validation**

What should the algorithm check to avoid errors when receiving input from a user?

Implementation 1 and 2 should both check whether the lists have common errors such as empty list and invalid characters, and check if the lists are sorted

**Checklist to guide your answer:**

| Implementation 1 | Implementation 2 |
| ----- | ----- |
| ~~Does the algorithm check if the list is empty? Does it handle invalid inputs (like letters instead of numbers)? Does it avoid crashing when inputs are unusual? Does it check that the list is sorted before using Linear Search?~~ | ~~Does the algorithm check if the list is empty? Does it handle invalid inputs (like letters instead of numbers)? Does it avoid crashing when inputs are unusual? Does it check that the list is sorted before using Binary Search?~~ |

### 

### **6\. Final Answer**

Based on your answers from 1 to 5, Which algorithm would you choose for this problem, and under what conditions would the other algorithm be more suitable? Summarize your answer

We would use Implementation 2 under the conditions of either wanting a faster process on larger numbers, or when showing a beginner a code and explaining it as we understand the algorithm thanks to its simple readability. While for Implementation 1, we would use this in the conditions of smaller numbers or when we have numbers that don’t need to be sorted.