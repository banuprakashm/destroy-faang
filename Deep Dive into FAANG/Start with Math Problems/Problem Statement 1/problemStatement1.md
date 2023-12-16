# Problem Statement 1
### Given an integer, check whether it is a palindrome or not.
### Sample Input & Output
- Input : 123 -> Output: Not a palindrome
- Output: 121 -> Output: Palindrome

### Solution
```python
def problemStatement1(inputValue):
    for i in range(0, len(inputValue)//2):
        if inputValue[i] != inputValue[len(inputValue)-i-1]:
            return False
    return True
inputData = "121"
if(problemStatement1(inputData) == True):
    print("Palindrome")
else:
    print("Not a palindrome")
```