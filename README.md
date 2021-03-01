# Machine_Learning
This is all material I have collected from course COMP**** in my university. I hope that it will save my time when I look for something in the future
## Class  in Python

```
# define a parent class
class my_parent(object):
     def __init__(self, my_var): # constructor
         self.member_var = my_var
         print(f'{self.__class__.__name__}.member_var is defined')

# define the child class
class my_child(my_parent):           
     def child_function(self):
         print(f'printing from child function the member variable with value {self.member_var}')
        
# now instantiate a child
child_obj = my_child(1) 
# output: my_child.member_var is defined

child_obj.child_function()
# output: printing from child function the member variable with value 1
```

## Numpy

```
import numpy as np
```

### Create array:
```
np.ones(5)
# output: array([1., 1., 1., 1., 1.])
```

```
np.zeros(5)
# output: array([0., 0., 0., 0., 0.])
```

Generate 1D, 2D and 3D array:

```
# generate random numbers
np.random.seed(4211)  # seed for reproducibility

x1 = np.random.randint(10, size=6)  # One-dimensional array
x2 = np.random.randint(10, size=(3, 4))  # Two-dimensional array
x3 = np.random.randint(10, size=(3, 4, 5))  # Three-dimensional array

print('x1', x1)
print('x2', x2)
print('x3', x3)
```

