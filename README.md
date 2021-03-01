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

