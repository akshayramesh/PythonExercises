```python
def new_function():
    print("You have entered the function")
    n1 = 100
    n2 = 99
    return n1,n2

p1,p2 = new_function()
print(p1, p2)
```

    You have entered the function
    100 99
    


```python
def new_function1(a1, a2):
    print("You have entered the function")
    n1 = 100 + a1
    n2 = 99 + a2
    return n1,n2

p1,p2 = new_function1(10, 20)
print(p1, p2)
```

    You have entered the function
    110 119
    


```python
##Find maximum of three numbers

def find_max(a, b, c):
    if a>b & a>c :
        return a
    elif b>a & b>c:
        return b
    else:
        return c
    
print(find_max(3,2,1))
print(find_max(20, 90, 40))
print(find_max(67, 89, 999))
print(find_max(67, 89, 9))
```

    3
    40
    999
    67
    


```python
###Find maximum of three numbers
###2nd variety

def find_max(a,b):
    if a<b:
        return b
    else:
        return a

    
print(find_max(find_max(4,5),19))
print(find_max(find_max(42,15),19))
print(find_max(find_max(41,53),19))


```

    19
    42
    53
    


```python
###Fibonacci series

def print_fibonacci(n):
    a = 0
    b = 1
    print(a)
    print(b)
    
    for i in range(2,n):
        c = a+b        
        a = b
        b = c
        print(c)
        
print(print_fibonacci(5))
```

    0
    1
    1
    2
    3
    None
    


```python
###Sum of numbers

def sum_of_numbers(numbers):
    total = 0
    for i in numbers:
        total += i
    return total
    
print(sum_of_numbers((1,2,3,4,5,6)))
```

    21
    


```python
### Reverse a string

def reverse_string(str):
    str_len = len(str)
    rev_str = ''
    while(str_len > 0):
        rev_str += str[str_len - 1]
        str_len -= 1
    return rev_str

    
print(reverse_string("Hello"))
```

    olleH
    


```python
### Factorial

def factorial(n):
    f = 1
    for i in range(1,n+1):
        f *= i
    return f

print(factorial(5))
```

    120
    


```python
### factorial using recursion

def factorial(n):
    if n == 1:
        return 1
    else:
        return n * factorial(n-1)
print(factorial(5))
```

    120
    


```python
### check whether a number is in a given range

def check_range(num, n1, n2):
    if num in range(n1, n2):
        return True
    else:
        return False

print(check_range(2, 1, 5))
print(check_range(20, 1, 5))
```

    True
    False
    
