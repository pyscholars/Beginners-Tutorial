# Conditional Statement

Conditional Statement in Python perform different computations or actions depending on whether a specific Boolean constraint evaluates to true or false. Conditional statements are handled by **`if ... elif ... else`** statements in python.

#### if Statement
**if** statement is used for decision making. It will run the body of code only IF the statement is satisfied or true. When you want to justify one condition while the other condition is not true, then you use **if** statement

```python
if expression:
    statement(s)
```

Above is the syntax for the if statement. Now let's see an example of an if statement in action.
We would use python to determine if a number is a positive number when that number is greater than 0.

<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><pre style="margin: 0; line-height: 125%"><span style="color: #0000DD; font-weight: bold">In [2]:</span> num <span style="color: #333333">=</span> <span style="color: #007020">input</span>(<span style="color: red">&quot;</span><span style="color: #666666; font-weight: bold; color: red">\n</span><span style="color: red">Enter a number: &quot;</span>)<br>        number <span style="color: #333333">=</span> <span style="color: #007020">int</span>(num)<br><br>        <span style="color: #008800; font-weight: bold">if</span> number <span style="color: #333333">&gt;</span> <span style="color: #0000DD; font-weight: bold">0</span>:<br>            <span style="color: #008800; font-weight: bold">print</span>(number, <span style="color: red">&quot;is a positive number.&quot;</span>)</pre></div>


Above we have created a variable num to receive a number from the user. After that we convert the input num to an integer, this is because the **input()** takes strings only while **>** works with  integers. Lets run the program and see the output.

<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><pre style="margin: 0; line-height: 125%"><span style="color: #fd9595; font-weight: bold">Out[2]:</span> Enter a number: <input type="text" value="7" disabled><br>        <span>7</span> <span>is</span> a positive number.</pre></div>


After running the program, we provided the number 7 and our output is 7 is a positive number.

#### if...else Statement

```python
if expression:
    statement(s)
else:
    statement(s)
```

Above is the syntax for the if...else statement. Now let's see an example of the if...else statement in action.

I believe we all are thinking of what if we provided a negative number, what should the output be? Well here we can get the response of if the number we provided is negative using the if….else statement.

Well here we can get the response of if the number we provided is negative using the if….else statement.  

<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><pre style="margin: 0; line-height: 125%"><span style="color: #0000DD; font-weight: bold">In [2]:</span> number <span style="color: #007020">input</span>(<span style="color: red">&quot;\nEnter a number: &quot;</span>)<br>        number <span style="color: #333333">=</span> <span style="color: #007020">int</span>(num)<br><br>        <span style="color: #008800; font-weight: bold">if</span> number <span style="color: #333333">&gt;</span> <span style="color: #0000DD; font-weight: bold">0</span>:<br>            <span style="color: #008800; font-weight: bold">print</span>(number, <span style="color: red">&quot;is a positive number.&quot;</span>)<br>        <span style="color: #008800; font-weight: bold">else</span>:<br>            <span style="color: #008800; font-weight: bold">print</span> (number, <span style="color: red">&quot;is a negative number.&quot;</span>)</pre></div>


Above we have added our else conditional statement to inform us if the number entered by the user is a negative number when a negative number is entered. Let’s take a look at the output when we enter a negative number. 

<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><pre style="margin: 0; line-height: 125%"><span style="color: #fd9595; font-weight: bold">Out[2]:</span> Enter a number: <input type="text" value="-5" disabled><br>        <span>-5</span> <span>is</span> a negative number.</pre></div>

As seen above that the output we get is from the else condition since the number -5 is a negative number.

Let's take a look at another scenario, I believe we all make use of apps that ask for our username and passwords when logging in.

<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><pre style="margin: 0; line-height: 125%"><span style="color: #0000DD; font-weight: bold">In [2]:</span> username <span style="color: #333333">=</span> <span style="color: #007020">input</span>(<span style="color: red">&quot;\nPlease enter username? &quot;</span>)<br>        password <span style="color: #333333">=</span> <span style="color: #007020">input</span>(<span style="color: red">&quot;\nPlease enter password &quot;</span>)<br><br>        <span style="color: #008800; font-weight: bold">if</span> username <span style="color: #333333">==</span> <span style="color: red">&#39;tina&#39;</span>:<br>            <span style="color: #008800; font-weight: bold">print</span>(<span style="color: red">&#39;\nHello Tina&#39;</span>)<br>        <span style="color: #008800; font-weight: bold">else</span>:<br>            <span style="color: #008800; font-weight: bold">print</span>(<span style="color: red">&#39;\incorrect username&#39;</span>)<br><br>        <span style="color: #008800; font-weight: bold">if</span> password <span style="color: #333333">==</span> <span style="color: red">&#39;swordfish&#39;</span><br>            <span style="color: #008800; font-weight: bold">print</span>(<span style="color: red">&#39;Access granted! Welcome Tina.&#39;</span>)<br>        <span style="color: #008800; font-weight: bold">else</span>:<br>            <span style="color: #008800; font-weight: bold">print</span>(<span style="color: red">&#39;incorrect password'</span>)</pre></div>


Above we have created a variable for username and password to receive the input tina as the username and swordfish as the password. From what we have if the username provided is tina the output would be Hello Tina and if it’s not (else) it gives the output incorrect username. Same goes for the password. Let's take a look at the output for both an incorrect input and a correct one.

<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><pre style="margin: 0; line-height: 125%"><span style="color: #fd9595; font-weight: bold">Out[2]:</span> Please enter username?: <input type="text" value="tina" disabled><br>        Please enter password:  <input type="text" value="catwoman" disabled><br>        Hello Tina<br>        incorrect password</pre></div>

As seen above we provided the correct username tina but gave a wrong password catwoman and that can be seen from the output we got. 

#### elif Statement
**elif** condition tells the program to print out the third condition or possibility when the other condition goes wrong or incorrect. The **elif** is short for else if. It allows the program to check for multiple expressions. For example if the condition for our **if** is False, it checks the condition of the next **elif** block and so on. If all the conditions are False, body of **else** is then executed.

```python
if expression:
    statement(s)
elif another expression:
    statement(s)
elif another expression:
    statement(s)
else:
    statement(s)
```

Let's take a look at an example

<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><pre style="margin: 0; line-height: 125%"><span style="color: #0000DD; font-weight: bold">In [2]:</span> num <span style="color: #333333">=</span> <span style="color: #007020">input</span>(<span style="color: red">&quot;\nEnter a number: &quot;</span>)<br>        number <span style="color: #333333">=</span> <span style="color: #007020">int</span>(num)<br><br>        <span style="color: #008800; font-weight: bold">if</span> number <span style="color: #333333">&gt;</span> <span style="color: #0000DD; font-weight: bold">0</span>:<br>            <span style="color: #008800; font-weight: bold">print</span>(number, <span style="color: red">&quot;is a positive number.&quot;</span>)<br>        <span style="color: #008800; font-weight: bold">elif</span> number <span style="color: #333333">==</span> <span style="color: #0000DD; font-weight: bold">0</span>:<br>            <span style="color: #008800; font-weight: bold">print</span>(number, <span style="color: red">&quot;is neither a positive nor negative number.&quot;</span>)<br>        <span style="color: #008800; font-weight: bold">else</span>:<br>            <span style="color: #008800; font-weight: bold">print</span>(number, <span style="color: red">&quot;is a negative number.&quot;</span>)</pre></div>


From what we can see above, we now have an elif condition to check and give an output if the user gives the number 0 which is neither positive nor negative. Let's take a look at the output.

<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><pre style="margin: 0; line-height: 125%"><span style="color: #fd9595; font-weight: bold">Out[2]:</span> Enter a number: <input type="text" value="0" disabled><br>        0 is neither a positive nor negative number.</pre></div>s

After running our program we receive an output from the elif condition because the user provided 0 as the number.


#### Nested if Statement
Do you know we can have a **`if...elif...else`** statement inside another **`if...elif...else`** statement?.
Yes!  This is called nesting in computer programming. Any number of these statements can be nested inside one another. But this can get confusing, so you must be avoided if we can. Let's look at an example.

<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><pre style="margin: 0; line-height: 125%">In [<span style="color: #0000DD; font-weight: bold">3</span>]: num <span style="color: #333333">=</span> <span style="color: #007020">float</span>(<span style="color: #007020">input</span>(<span style="color: red">&quot;Enter a number: &quot;</span>)<br><br>        <span style="color: #008800; font-weight: bold">if</span> num <span style="color: #333333">&gt;=</span> <span style="color: #0000DD; font-weight: bold">0</span>:<br><br>            <span style="color: #008800; font-weight: bold">if</span> num <span style="color: #333333">==</span> <span style="color: #0000DD; font-weight: bold">0</span>:<br>                <span style="color: #008800; font-weight: bold">print</span>(number,<span style="color: red">"is neither positive nor negative number."</span>)<br>             <span style="color: #008800; font-weight: bold">else</span>:<br>                <span style="color: #008800; font-weight: bold">print</span>(num, <span style="color: red">&quot;is a positive number.&quot;</span>)<br>        <span style="color: #008800; font-weight: bold">else</span>:<br>            <span style="color: #008800; font-weight: bold">print</span> (num, <span style="color: red">&quot;is a negative number.&quot;</span>)</pre></div>


Above is an example of a nested if statement. You can try and run it, yes it looks similar to our elif example but this is a different approach. You can notice that here we converted the user’s input to a float() using a different style from the int() we used previously.

