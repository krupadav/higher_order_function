# higher_order_function:
3 types of higher order functions:
 1. map
 2. filter
 3. reduce
1. map(func,iterable): The function inside a map will be applied on each element from iterable.
"when we got the output in the form of object then to see actual values typecast the object
print(list(map(lambda num:num*num, ls))) # this lambda function will be applied on each element of ls"
2. Filter(func,iterable) used to filter out the values based on condition given inside a function it will return results for only True instances filter will give a original sequence or may be sub-sequence, filter will check this condition and selects values from sequence where it returns True.
3. Reduce: used to reduce the sequence into single object
Example: sum,greater no,
Reduce is not directly present like map and filter it is present in functools moduleso we need to import reduce
Syntax: reduce(function,sequence) #in case of reduce we need not to typecast
from functools import reduce
k = [12,45,3,67,89,90,1,23,44,68,22] # find out largest number
print(reduce(lambda x,y: x if x>y else y,k))
