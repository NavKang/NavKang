Contents:

1. Creating Virtual Enviroment, Pydocs, MakeFile

2. Quick Tips

3. String Functions

4. Sequence Operations and Functions: Len(), max(), min()

5. Iterators

6. Lists/Dictionaries/Tuples

7. 

8.

9. Funtions

10. Classes (OOP)

#### Python Ramble
Practice as much python as you can. Build small basic programs and build on them. There are plenty of very good resources online to learn python. Some of the books I highly recommend are:

+ Python Crash Course

+ Head First Python

+ The Coder's Apprentice

*To become a good programmer, you must practice. This is the advice I live by, and to become a good programmer is my goal.*
<br><hr>

#### Python Useful  
##### Create and Activate Virtual Enviroment: &nbsp;  
1. python3 -m venv   <select dir name> &nbsp; 

2. . ./<name of virtual enviroment>/bin/activate &nbsp; 

Using Pydocs:

pdoc3 <python file name>

pdoc3 -html <.py name> ( can also do -pdf for output)

file://home/<dirname>/<.py name>  --to access in browser



Make File:

make -- provides several options 

make venv --creates virtual enviroment

make prereqs -- auto pip installs libraries needed

make test --runs tests



Quick Tips in Python:



Separator - used in print function:

        eg. print("N", "A", "V", sep="--")   result= N--A--V

        eg. print("Nav", "555", sep="@") result= nav@555



Decimal places format:

        eg. 458.541315 to 458.54

        print(f"{458.541315: .2f3")



Create multiple strings from one input call:

       eg. str1, str2, str3 = input("Enter three strings").split()

       print(str1, str2, str3)



Check if a file is empty:

       eg. import OS; print(os.stat("test.txt").st_size==0



Python modules stored on computer:

       eg. import sys ; sys_path



Print per line:

      eg. print(end=' ')



String Functions:

        

       eg: text = "Welcome to Navs Site"

             nums = "98765"



Find Text:

text.find("Navs") 

text.find("Site")



Validation Checks:

text.isalpha()

text.isdigits()

nums.isdigit()



Concatenation:

' '.join((text,nums))

'   '.join((text,numbers))



Case change:

text.upper()

text.lower()



Splitting String:

text.split('  ')



Substitution:

text.replace("Navs", "Vans")



Stripping:

text.rstrip()

text.lstrip()

text.strip()



Sequence Operations and Functions:

len() --find length of list using this function

max()

min()

sum()

sorted()

reversed()
