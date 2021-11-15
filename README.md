# Python-Cheatsheet
Common algorithms, tips and tricks that a pythoneer or a pythonista might need during the adventures or coding interviews.
<br/><br/><br/>
## Reverse an Integer
---

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
---

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
