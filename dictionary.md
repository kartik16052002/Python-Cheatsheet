# empty dict
user = {}

# with values
user = {
    "name": "Kartik",
    "age": 22,
    "is_admin": False
}

# using dict()
user = dict(name="Kartik", age=22)

# from list of pairs
pairs = [("a", 1), ("b", 2)]
d = dict(pairs)  # {'a': 1, 'b': 2}



user["name"]      # 'Kartik'
user.get("age")   # 22
user.get("city", "unknown")  # default if key missing -> 'unknown'

# update or add key
user["age"] = 23
user["city"] = "Udaipur"


user.pop("age")         # removes and returns value
user.popitem()          # removes last added (random in older versions)
del user["city"]        # delete by key
user.clear()            # empty the dict



info = {"a": 1, "b": 2, "c": 3}

# get keys, values, items
info.keys()     # dict_keys(['a','b','c'])
info.values()   # dict_values([1,2,3])
info.items()    # dict_items([('a',1),('b',2),('c',3)])

# copy or merge
new_info = info.copy()
info.update({"d": 4})   # merges new data


for key in info:
    print(key, info[key])

# or more Pythonic
for k, v in info.items():
    print(f"{k} -> {v}")


# squares of numbers
squares = {x: x**2 for x in range(1, 6)}  
# {1:1, 2:4, 3:9, 4:16, 5:25}

# filtering
even_squares = {k:v for k,v in squares.items() if v % 2 == 0}


[W3Schools][https://www.w3schools.com/python/python_dictionaries.asp]
[GFG][https://www.geeksforgeeks.org/python/python-dictionary/]