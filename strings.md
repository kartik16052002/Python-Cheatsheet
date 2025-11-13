# single, double, or triple quotes
s1 = 'hello'
s2 = "world"
s3 = '''multi
line string'''

# empty string
empty = ""

# escape characters
msg = "He said, \"Python is fun!\""

## if you want to include escape charater

msg = "........//............"
OR
msg = r"........./........."

Below code is valid because '/' works here also
msg = r"......../"........"
In the above msg '/' will be visible

name = "Kartik"

len(name)           # 6
name[0]             # 'K'
name[-1]            # 'k'
name[1:4]           # 'art'
name[::-1]          # reverse -> 'kitraK'


# String Methods (most used ones)
txt = "  hello world  "

txt.upper()        # '  HELLO WORLD  '
txt.lower()        # '  hello world  '
txt.strip()        # removes spaces -> 'hello world'
txt.replace("world", "Python")  # '  hello Python  '

txt.startswith("  h")   # True
txt.endswith("ld  ")    # True

txt.find("lo")      # 3 (index)
txt.count("l")      # 3

# Joining and splitting

# split string into list
s = "a,b,c".split(",")      # ['a','b','c']

# join list into string
",".join(["a", "b", "c"])   # 'a,b,c'

# split by spaces
"hi there world".split()    # ['hi','there','world']


# Formatting Strings

name = "Kartik"
age = 22

# f-string (modern and clean)
msg = f"My name is {name} and I am {age}"

# format() method
msg2 = "My name is {} and I am {}".format(name, age)

# old-style
msg3 = "My name is %s and I am %d" % (name, age)


# Checking Content

word = "Python3"

word.isalpha()     # False (because of 3)
word.isdigit()     # False
"123".isdigit()    # True
word.isalnum()     # True (letters + digits)
"python".islower() # True
"HELLO".isupper()  # True


# looping

for ch in "Hi!":
    print(ch)

# reverse quickly
rev = "".join(reversed("python"))

# count vowels
vowels = sum(ch.lower() in "aeiou" for ch in "Kartik")

# References

[W3Schools](https://www.w3schools.com/python/python_strings.asp)
[DevDocs](https://docs.python.org/3.14/whatsnew/3.14.html#whatsnew314-template-string-literals)