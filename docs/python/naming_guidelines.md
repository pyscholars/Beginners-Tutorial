# Naming Guidelines

In Python there are few guidelines we follow when naming variables, classes and functions

#### Variables
In naming your variables you must start with a letter or an underscore (name, _name)
You should not use words that are too long. Let's look at some good variable names and bad ones also.

| Good       | Bad                    |
|------------|------------------------|
| user       | my_list                |
| first_name | name_of_the _students  |
| username   |  O, i                  |

Readability is also important when giving a name. Which of the following is easiest to read? 

    a) first_name 
    b) firstname

I’m sure we would all select A meaning readability is very important.

Take note that names are case sensitive, this means that User_Name and user_name are different names. Also Python reserved words can’t be used as a variable name. 

|        |          |         |          |
|--------|----------|---------|----------|
| FALSE  | assert   | del     | for      |
| None   | break    | elif    | from     |
| TRUE   | class    | else    | global   |
| and    | continue | except  | if       |
| As     | def      | finally | import   |
| in     | or       | raise   | while    |
| is     | pass     | return  | with     |
| lambda | not      | try     | Yield    |
|        |          |         | nonlocal |

#### Functions

Naming a function follows similar rules as we learnt about naming a variable, the only thing is that a function should convey what it does. For example def greet from the function we created earlier in this tutorial is very basic and does only one thing which is to greet as the name implies.

#### Classes 

Naming classes we start each word with a capital letter. You are not to separate words with underscores. This style is called camel case.
 **Model**,  **MyClass**