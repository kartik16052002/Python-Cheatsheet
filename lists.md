

# Empty list
nums = []

# With elements
fruits = ["apple", "banana", "mango"]

# Mixed types
info = ["Kartik", 25, True]

# From iterable
chars = list("hello")        # ['h','e','l','l','o']
numbers = list(range(1, 6))  # [1,2,3,4,5]

a = ["a", "b", "c", "d"]

# Indexing
a[0]    # 'a'
a[-1]   # 'd'  (last item)

# Slicing (start:stop:step)
a[1:3]     # ['b', 'c']
a[:2]      # ['a', 'b']
a[::2]     # ['a', 'c']
a[::-1]    # reversed -> ['d','c','b','a']


lst = [3, 1, 4]

lst.append(2)        # add single item -> [3,1,4,2]
lst.extend([5, 6])   # add multiple -> [3,1,4,2,5,6]
lst.insert(1, 99)    # insert at index -> [3,99,1,4,2,5,6]

lst.remove(99)       # remove first matching value
val = lst.pop()      # pop last (or pop(i) to remove index i)
lst.clear()          # empty the list

# search & info
idx = lst.index(4)   # index of first 4 (ValueError if not found)
cnt = lst.count(4)   # how many 4s

# order & copy
lst.sort()           # sorts in-place
sorted_lst = sorted(lst)  # returns new sorted list
lst.reverse()        # reverse in-place
shallow = lst.copy() # shallow copy


names = ["alice", "bob", "carol"]

# simple loop
for n in names:
    print(n)

# with index
for i, n in enumerate(names):
    print(i, n)

# list comprehension (quick transform)
upper = [n.upper() for n in names]   # ['ALICE','BOB','CAROL']

# filter & map style
evens = [x for x in range(10) if x % 2 == 0]

mat = [
    [1, 2, 3],
    [4, 5, 6]
]

mat[0][1]   # 2
# loop rows
for row in mat:
    for val in row:
        print(val)

# References

[W3Schools][https://www.w3schools.com/python/python_lists.asp]
[GFG][https://www.geeksforgeeks.org/python/python-lists/]