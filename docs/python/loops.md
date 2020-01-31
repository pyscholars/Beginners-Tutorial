# Loops

A loop in a computer program is an instruction that repeats until a specified condition is reached. In a loop structure, the loop asks a question. If the answer requires action, it is executed. The same question is asked again and again until no further action is required. Each time the question is asked is called an iteration.

#### for loop
A **for** loop is a loop that runs for a preset number of times. It is often used when you have a piece of code which you want to repeat "n" number of times. 

```python
for value in sequence:
    statement(s)
```

Above we see the for loop syntax, Here, val is the variable that takes the value of the item inside the sequence on each iteration. Let’s now take a look at an example.

<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><pre style="margin: 0; line-height: 125%"><span style="color: #0000DD; font-weight: bold">In [2]:</span> months <span style="color: #333333">=</span> [<span style="color: red">&quot;Jan&quot;</span>, <span style="color: red">&quot;Feb&quot;</span>, <span style="color: red">&quot;Mar&quot;</span>,<span style="color: red">&quot;April&quot;</span>, <span style="color: red">&quot;May&quot;</span>,<span style="color: red">&quot;June&quot;</span>]<br><br>        <span style="color: #008800; font-weight: bold">for</span> month <span style="color: #008800; font-weight: bold">in</span> months:<br>            <span style="color: #008800; font-weight: bold">print</span>(month)</pre></div>


Above, we have a list of the first 6 months of the year. We also have a for loop that reads, for every element that we assign the variable month, in the list months, print out the variable month.

<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><pre style="margin: 0; line-height: 125%"><span style="color: #fd9595; font-weight: bold">Out[2]:</span> Jan<br>        Feb<br>        Mar<br>        April<br>        May<br>        June</pre></div>

And above we have the output of our loop.

#### while loop

The while loop is used to repeat a specific block of code an unknown number of times, until a condition is met. Let’s now take a look at an example.

<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><pre style="margin: 0; line-height: 125%"><span style="color: #0000DD; font-weight: bold">In [2]:</span> numbers <span style="color: #333333">=</span> <span style="color: #0000DD; font-weight: bold">0</span><br><br>        <span style="color: #008800; font-weight: bold">while</span> numbers <span style="color: #333333">&lt;=</span> <span style="color: #0000DD; font-weight: bold">10</span>:<br>            <span style="color: #008800; font-weight: bold">print</span>(numbers)<br>            numbers <span style="color: #333333">+=</span> <span style="color: #0000DD; font-weight: bold">1</span></pre></div>


Above we have a loop that starts from 0 and increases by 1 until it is equal to 10. This means that while numbers is less than or equal to 10, print out numbers. Let’s take a look at the output

<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><pre style="margin: 0; line-height: 125%"><span style="color: #fd9595; font-weight: bold">Out[2]:</span> 0<br>        1<br>        2<br>        3<br>        4<br>        5<br>        6<br>        7<br>        8<br>        9<br>        10</pre></div>

Above we can see that the outputs we got are the numbers from 0 to 10. 

The same results we got from our while loop can be gotten in Python using the **`range()`** function. The **`range()`** function returns a sequence of numbers, starting from 0 by default, and increments by 1 (by default), and ends at a specified number. Let's take a look at an example of that.

<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><pre style="margin: 0; line-height: 125%"><span style="color: #0000DD; font-weight: bold">In [2]:</span> <span style="color: #008800; font-weight: bold">for</span> numbers <span style="color: #000000; font-weight: bold">in</span> <span style="color: #007020">range</span>(<span style="color: #0000DD; font-weight: bold">0</span>,<span style="color: #0000DD; font-weight: bold">10</span>):<br>            <span style="color: #008800; font-weight: bold">print</span>(numbers)<br><br><br><span style="color: #fd9595; font-weight: bold">Out[2]:</span> 0<br>        1<br>        2<br>        3<br>        4<br>        5<br>        6<br>        7<br>        8<br>        9</pre></div>

So above we can see that the outputs we got are the numbers from 0 to 9. Some would be wondering why in the while loop we got 0 - 10 and here 0 - 9, this is be in our while loop we used the condition less than or equal to 10, this makes 10 included in the output displayed.


#### Break and Continue statements

With the **break** statement we can stop the loop before it has looped through all the items,

<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><pre style="margin: 0; line-height: 125%"><span style="color: #0000DD; font-weight: bold">In [2]:</span> numbers <span style="color: #333333">=</span> <span style="color: #0000DD; font-weight: bold">0</span><br><br>        <span style="color: #008800; font-weight: bold">while</span> numbers <span style="color: #333333">&lt;=</span> <span style="color: #0000DD; font-weight: bold">10</span>:<br>            <span style="color: #008800; font-weight: bold">if</span> numbers <span style="color: #333333">=</span> <span style="color: #0000DD; font-weight: bold">5</span>:<br>                <span style="color: #008800; font-weight: bold">break</span><br>            <span style="color: #008800; font-weight: bold">print</span> (numbers)<br>            numbers <span style="color: #333333">+=</span> <span style="color: #0000DD; font-weight: bold">1</span><br><br><br><span style="color: #fd9595; font-weight: bold">Out[2]:</span> 0<br>        1<br>        2<br>        3<br>        4</pre></div>


Above we included a **break** statement that if our loop get to 5 it should exit, and that can be seen in the output.

With **continue** statement we can stop the current iteration of the loop, and continue with the next

<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><pre style="margin: 0; line-height: 125%"><span style="color: #0000DD; font-weight: bold">In [2]:</span> months <span style="color: #333333">=</span> [<span style="color: red">&quot;Jan&quot;</span>, <span style="color: red">&quot;Feb&quot;</span>, <span style="color: red">&quot;Mar&quot;</span>, <span style="color: red">&quot;April&quot;</span>, <span style="color: red">&quot;May&quot;</span>, <span style="color: red">&quot;June&quot;</span>]<br><br>        <span style="color: #008800; font-weight: bold">for</span> month <span style="color: #000000; font-weight: bold">in</span> months:<br>            <span style="color: #008800; font-weight: bold">if</span> month <span style="color: #333333">==</span> <span style="color: red">&quot;April&quot;</span>:<br>                <span style="color: #008800; font-weight: bold">continue</span><br>            <span style="color: #008800; font-weight: bold">print</span>(month)<br>        <span style="color: #008800; font-weight: bold">print</span>(<span style="color: red">&quot;</span><span style="color: #666666; font-weight: bold; color: red">\n</span><span style="color: red">The end&quot;</span>)<br><br><span style="color: #fd9595; font-weight: bold">Out[2]:</span> Jan<br>        Feb<br>        Mar<br>        May<br>        June<br>        The end</pre></div>


Above we have used the continue statement to skip “April”, and return to the for loop statement. In the output we can see that April isn’t part of the results.






