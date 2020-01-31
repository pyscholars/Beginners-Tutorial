# Project on a Biography Bot

We would build a project with to make a Biography bot that asks for your input and gives back a summarized story using the inputs you give.

We would create a bot like app that you can name after yourself or a name you love.
We would also make use of the datetime module in python. The datetime module supplies classes for manipulating dates and times in both simple and complex ways. We would need that because we would add some delays during the output of the project.

```python 
from datetime import datetime
import time

ai = "Bill",
fname = input("Please what is your first name? ")
lname = input("Please what is your last name? ")
gender = input("Are you male or female? ")
if gender.lower() == 'male':
    a = "Mr",
    b = "he",
    c = "He",
    d = "boy",
    e = "handsome",
    f = "his",
    g = "man",
elif gender.lower() == 'female':
    a = "Ms",
    b = "she",
    c = "She",
    d = "girl",
    e = "pretty",
    f = "her",
    g = "lady",
else:
    g ="not specified",
dob = input("Enter DOB, use dd/mm/yyyy format: ")
dob = datetime.strptime(dob, '%d/%m/%Y')
hobbies = input ("What are you hobbies? ")
school = input ("Where do you school? ")

time.sleep(2)
print("\n\nHello %s" % (a), fname, "my name is %s" % (ai),) 
time.sleep(3)
#I am your Personal Assistant and have a story for you (THE NAME OF THE USER).
print("I am your Personal Assistant and have a story for you, %s" % (fname),)
time.sleep(4)
print("Sit back and enjoy.\n\n") 
time.sleep(6)
print("In the year %s" % (dob.year), "a family gave birth to a beautiful baby %s" % (d),
 "called %s" % (fname),".")
time.sleep(6)
print("%s" % (fname), "was so playful and grew to be a %s" % (e), "young %s" % (g),)
time.sleep(6)
print("%s" % (c), "loves %s" % (hobbies), "and currently schools in %s" % (school),".")
time.sleep(8)
print("%s" % (c), "thinks I don't know that %s" % (b), "is %d" % ((datetime.today() - dob).days/365), 
"years, but by only providing her date of birth I can get that 😉.")
time.sleep(8)
print("All I needed were few calculations and tah da!")
time.sleep(9)
print("And in case you are wondering, %s" % (f), " full name is %s" % (a), (fname), (lname),)
time.sleep(9)
print("\nWell thanks so much for your time, looking forward to getting to know you better 😊")
time.sleep(8)
print("\nBye,\n%s" % (ai),)
x=input("---------------------------------")
```