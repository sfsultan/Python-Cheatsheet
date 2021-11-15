# Python-Cheatsheet
Common algorithms, tips and tricks that a pythoneer or a pythonista might need during the adventures or coding interviews.
<br/><br/><br/>
## Reverse an Integer

```python
def reverse_integer(x):

    '''
    Returns a reverse of a provided integer. Takes into account negative numbers as well.
    '''

    string_int = str(x)

    if string_int[0] == '-':
        return int('-' + string_int[:0:-1])
    else:
        return int(string_int[::-1])
```
<br/><br/><br/>
## Move Zeros to the end of the array

```python

def move_zeros(num_list):

    '''
    Returns a list where all the zeros will be moved to the end of the list.
    '''

    for i in num_list:
        if 0 in num_list:
            num_list.remove(0)
            num_list.append(0)
    return num_list
```
<br/><br/><br/>

## Check if a string is valid Palindrome

```python
def check_palindrome(input_string):

    '''
    Returns True or False when checking if the provided string is a valid Palindrome (string == reverse of the string)
    '''
    if t == t[::-1]:
        return True
```
<br/><br/><br/>

## Check if a string can be made a valid Palindrome by removing any one of the characters

```python
def make_palindrome(input_string):

    '''
    Returns True or False when checking if the provided string is a valid Palindrome (string == reverse of the string)
    '''
    for i in range(len(input_string)):
        t = input_string[:i] + input_string[i+1:]

        if t == t[::-1]:
            return True

    return input_string == input_string[::-1]
```
<br/><br/><br/>

## Generate all the Prime Numbers from 2 to an input number

```python
def generate_primes(num):

    '''
    Returns a list of prime numbers from 2 to a given input number
    '''
    primes = []
    for num in range(n):
        if num > 1:
            for i in range(2, num):
                if (num % i) == 0:
                    break
            else:
                primes.append(num)
    return primes
```
