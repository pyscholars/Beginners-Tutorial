# Data types

### Numbers
Python supports two types of numbers - Integers and floating point numbers

<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><pre style="margin: 0; line-height: 125%"><span style="color: #0000DD; font-weight: bold">In [2]:</span> myint <span style="color: #333333">=</span> <span style="color: #0000DD; font-weight: bold">6</span><br>        myfloat <span style="color: #333333">=</span> <span style="color: #6600EE; font-weight: bold">6.0</span><span style="color: #008800; font-weight: bold"><br><br>        print</span>(myint)<span style="color: #008800; font-weight: bold"><br>        print</span>(myfloat)
<br><span style="color: #fd9595; font-weight: bold">Out[2]:</span> <span>6</span> <br>        <span>6.0</span>
</pre></div>



As seen above integers are whole numbers as known by students, there is effectively no limit to how long an integer value can be. While float numbers are decimal numbers as known in maths to student

| Type    | Format  | Description                                                              |
|---------|---------|--------------------------------------------------------------------------|
| int     | a=10    | Signed Integer                                                           |
| long    | a=345L  | (L) Long integers, they can also be represented in octal and hexadecimal |
| float   | a=45.67 | (.) Floating point real values                                           |
| complex | a=3.14J | (J) Contains integer in the range 0 to 255.                              |

#### Strings
A string in Python is a sequence of characters. It is a derived data type. A character is simply a symbol. For example, the English language has 26 characters.

<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><pre style="margin: 0; line-height: 125%"><span style="color: #0000DD; font-weight: bold">In [2]:</span> <span style="color: #007020">str</span> <span style="color: #333333">=</span> <span style="color: red">&quot;This is a string&quot;</span><br><br>        <span style="color: #008800; font-weight: bold">print</span> (<span style="color: #007020">str</span>)      <span style="color: #888888"># Prints complete string</span><br>        <span style="color: #008800; font-weight: bold">print</span> (<span style="color: #007020">str</span>[<span style="color: #0000DD; font-weight: bold">0</span>])   <span style="color: #888888"># Prints first character of the string</span><br>        <span style="color: #008800; font-weight: bold">print</span> (<span style="color: #007020">str</span>[<span style="color: #0000DD; font-weight: bold">2</span>:<span style="color: #0000DD; font-weight: bold">5</span>]) <span style="color: #888888"># Prints characters starting from 3rd to 5th</span><br>        <span style="color: #008800; font-weight: bold">print</span> (<span style="color: #007020">str</span>[<span style="color: #0000DD; font-weight: bold">2</span>:<span style="color: #0000DD; font-weight: bold">1</span>)  <span style="color: #888888"># Prints string starting from 3rd character</span><br>        <span style="color: #008800; font-weight: bold">print</span> (<span style="color: #007020">str</span> <span style="color: #0000DD; font-weight: bold">2</span>)    <span style="color: #888888"># Prints string two times</span><br>        <span style="color: #008800; font-weight: bold">print</span> (<span style="color: #007020">str</span> <span style="color: #333333">+</span> <span style="color: red">&quot;ADD THIS&quot;</span>) <span style="color: #888888"># Prints concatenated string</span><br>
<span style="color: #fd9595; font-weight: bold">Out[2]:</span> This <span>is</span> a string
        T
        <span>is</span>
        <span>is</span> <span>is</span> a string
        This <span>is</span> a string This <span>is</span> a string
        This <span>is</span> a stringADD THIS
</pre></div>


Python uses single quotes **'** double quotes **"** and triple quotes **"""** to denote literal strings. Only the triple quoted strings **"""** also will automatically continue across the end of line statement.

<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><pre style="margin: 0; line-height: 125%"><span style="color: #0000DD; font-weight: bold">In [2]:</span> firstName <span style="color: #333333">=</span> <span style="color: red">&#39;mannie&#39;<br>        </span>last Name <span style="color: #333333">=</span> <span style="color: red">&quot;young&quot;<br>        </span>message <span style="color: #333333">=</span> <span style="color: red">&quot;&quot;&quot;This shows a string that will span across multiple </span><br>       <span style="color: red"> lines Using newline characters and no spaces for the next lines. </span><br>       <span style="color: red"> The end of lines within this string also count as a newline when </span><br>       <span style="color: red"> printed&quot;&quot;&quot;</span><br><br>        <span style="color: #008800; font-weight: bold">print</span> (firstName)<br>        <span style="color: #008800; font-weight: bold">print</span> (lastName)<br>        <span style="color: #008800; font-weight: bold">print</span> (message)<br><br><span style="color: #fd9595; font-weight: bold">Out[2]:</span> mannie<br>       <span> young </span><br>        <span>This shows a string that will span across multiple lines
</span>        <span>Using newline characters and no spaces for the next lines. </span><br>        <span>The end of lines within this string also count as a newline when </span><br>        <span>printed</span>
</pre></div>


Python can use a special syntax to format multiple strings and numbers. We would cover the string formatter here briefly because it is seen often and it is important to recognize the syntax.

<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><pre style="margin: 0; line-height: 125%"><span style="color: #0000DD; font-weight: bold">In [2]:</span> <span style="color: #008800; font-weight: bold">print</span> (<span style="color: red">&quot;My name is (). I love to {}&quot;</span><span style="color: #333333">.</span>format(<span style="color: red">&quot;Mannie&quot;</span>, <span style="color: red">&quot;code&quot;</span>))<br><br><span style="color: #fd9595; font-weight: bold">Out[2]:</span> My name <span>is</span> Mannie, I love to code
</pre></div>


The **{}** are placeholders that are substituted by Mannie and code in the final string. This compact syntax is meant to keep the code more readable and compact. Python is currently transitioning to the format syntax above.

Deleting a string entirely is possible using the keyword **del**. So if we want to delete lastname we simply do **del** lastname

#### List
Lists are a very useful variable type in Python. A list can contain a series of values. List variables are declared by using brackets **[ ]** following the variable name. Yes Lists are exactly what you think they are: objects which are lists of other objects.

<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><pre style="margin: 0; line-height: 125%"><span style="color: #0000DD; font-weight: bold">In [2]:</span> home <span style="color: #333333">=</span> []    <span style="color: #888888"># This is a blank list variable</span><br>        names <span style="color: #333333">=</span> [<span style="color: red">&quot;Smith&quot;</span>, <span style="color: red">&quot;Ruth&quot;</span>, <span style="color: red">&quot;Rio&quot;</span>) <span style="color: #888888"># list creates a list names.</span><br>        marks <span style="color: #333333">=</span> [<span style="color: #0000DD; font-weight: bold">90</span>, <span style="color: #0000DD; font-weight: bold">88</span>, <span style="color: #0000DD; font-weight: bold">87</span>] <span style="color: #888888"># lists can have different data types.</span>
</pre></div>


So as seen above, we have created lists for home which is an empty list, names and marks! What can we do with it? 

<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><pre style="margin: 0; line-height: 125%"><span style="color: #0000DD; font-weight: bold">In [2]:</span> <span style="color: #008800; font-weight: bold">print</span> (<span style="color: #007020">len</span>(names))<br>        <span style="color: #008800; font-weight: bold">print</span> (names[<span style="color: #0000DD; font-weight: bold">1</span>])<br>        <span style="color: #008800; font-weight: bold">print</span> (marks[<span style="color: #0000DD; font-weight: bold">0</span>:<span style="color: #0000DD; font-weight: bold">2</span>])<br><br><span style="color: #fd9595; font-weight: bold">Out[2]:</span> <span>3</span><br>        <span>Ruth</span><br>        <span>[90, 88]</span>
</pre></div>


Above we used the `len()` function to can give us a number of objects in the list names. We also returned the value at index 1 of names, which is 'Ruth'. Note that The list index starts at zero.
You can add items to a list, we use the **append** function. A function is a chunk of code that tells Python to do something. In this case, append adds an item to the end of a list.

<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><pre style="margin: 0; line-height: 125%"><span style="color: #0000DD; font-weight: bold">In [2]:</span> home <span style="color: #333333">=</span> []    <span style="color: #888888"># This is a blank list variable</span><br>        names <span style="color: #333333">=</span> [<span style="color: red">&quot;Smith&quot;</span>, <span style="color: red">&quot;Ruth&quot;</span>, <span style="color: red">&quot;Rio&quot;</span>] <span style="color: #888888"># list creates a list names.</span><br>        marks <span style="color: #333333">=</span> [<span style="color: #0000DD; font-weight: bold">90</span>, <span style="color: #0000DD; font-weight: bold">88</span>, <span style="color: #0000DD; font-weight: bold">87</span>] <span style="color: #888888"># lists can have different data types.</span></pre></div>

We would try to add a new name Anthony to our list names.

<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><pre style="margin: 0; line-height: 125%"><span style="color: #0000DD; font-weight: bold">In [2]:</span> names<span style="color: #333333">.</span>append(<span style="color: red">&#39;Anthony'</span>)</pre></div>


Now lets print out our list to see the changes.

<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><pre style="margin: 0; line-height: 125%"><span style="color: #0000DD; font-weight: bold">In [2]:</span> <span style="color: #008800; font-weight: bold">print</span>(names)<br><br><span style="color: #fd9595; font-weight: bold">Out[2]:</span> [<span>&#39;Smith&#39;</span>, <span>&#39;Ruth&#39;</span>, <span>&#39;Rio&#39;</span>, <span>&#39;Anthony&#39;</span>]</pre></div>


Now we can see that we now have Anthony included in the list names. 

We can also remove a name from the list, and to do this we would use the **del** command (short for delete). 

For example, to remove the third item in the names list, Rio, we would do this:

<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><pre style="margin: 0; line-height: 125%"><span style="color: #0000DD; font-weight: bold">In [2]:</span> <span style="color: #008800; font-weight: bold">del</span> names [<span style="color: #0000DD; font-weight: bold">2</span>]</pre></div>

Now lets print out our list to see the changes.

<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><pre style="margin: 0; line-height: 125%"><span style="color: #0000DD; font-weight: bold">In [2]:</span> <span style="color: #008800; font-weight: bold">print</span>(names)<br><br><span style="color: #fd9595; font-weight: bold">Out[2]:</span> [<span>&#39;Smith&#39;</span>, <span>&#39;Ruth&#39;</span>, <span>&#39;Anthony&#39;</span>]</pre></div>

Now we can see that Rio has been deleted from the list names. 

> Instructor should remind the scholars the positions start at zero, so names[2] actually refers to the third item in the list.

# Tuples
Tuples are a group of values like a list and are manipulated in similar ways. But, tuples are fixed in size once they are assigned. A tuple consists of a number of values separated by commas. The main differences between lists and tuples are: Lists are enclosed in brackets **[ ]** and their elements and size can be changed, while tuples are enclosed in parentheses **( )** and cannot be updated. 

<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><pre style="margin: 0; line-height: 125%"><span style="color: #0000DD; font-weight: bold">In [2]:</span> home_tuple <span style="color: #333333">=</span> ()    <span style="color: #888888"># This is a blank tuple variable</span><br>        names <span style="color: #333333">=</span> (<span style="color: red">&quot;Anthony&quot;</span>,<span style="color: red">&quot;Abigail&quot;</span>,<span style="color: red">&quot;Michael&quot;</span>) <span style="color: #888888">#creates tuple of names</span><br>        marks <span style="color: #333333">=</span> (<span style="color: #0000DD; font-weight: bold">90</span>, <span style="color: #0000DD; font-weight: bold">88</span>, <span style="color: #0000DD; font-weight: bold">87</span>) <span style="color: #888888"># tuples contain that integers.</span></pre></div>

So as seen above, we have created tuples for home which is an empty list, names and marks!

<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><pre style="margin: 0; line-height: 125%"><span style="color: #0000DD; font-weight: bold">In [2]:</span> <span style="color: #008800; font-weight: bold">print</span> (<span style="color: #007020">len</span>(home_tuple))<br>        <span style="color: #008800; font-weight: bold">print</span> (<span style="color: #007020">len</span>(names))<br>        <span style="color: #008800; font-weight: bold">print</span> (names)<br>        <span style="color: #008800; font-weight: bold">print</span> (<span style="color: red">&#39;3rd mark: &#39;</span>, marks[<span style="color: #0000DD; font-weight: bold">2</span>])<br><br><span style="color: #fd9595; font-weight: bold">Out[2]:</span> <span>0</span><br>        <span>3</span><br>        <span>('Anthony', 'Abigail', 'Michael')</span><br>        <span>3rd mark: 93</span></pre></div>

Above we used the `len()` function to can give us a number of objects in the **tuple** home_tuple, notice the output is 0 since the tuple is empty. We also returned the value at index 2 of marks, which is **93**. Note that The list index starts at zero.

#### Dictionary
In Python a dictionary is a collection of things, like lists and tuples. The difference between dictionaries and lists or tuples is that each item in a dictionary has a key and a corresponding value. 

Creating a dictionary is as simple as placing items inside curly braces {} separated by comma. An item has a key and the corresponding value expressed as a pair, key: value. While values can be of any data type and can repeat, keys must be of immutable type (string, number or tuple with immutable elements) and must be unique.

Now lets create a dictionary called student:

<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><pre style="margin: 0; line-height: 125%"><span style="color: #0000DD; font-weight: bold">In [2]:</span> student <span style="color: #333333">=</span> {<span style="color: red">&#39;Name&#39;</span>: <span style="color: red">&#39;Ernie&#39;</span>, <span style="color: red">&#39;Age&#39;</span>: <span style="color: #0000DD; font-weight: bold">16</span>, <span style="color: red">&#39;Class&#39;</span>: <span style="color: red">&#39;First&#39;</span>}</pre></div>


As seen above have created a dictionary student with the keys Name, Age and Class and also they have the values  Ernie, 16 and First respectively.

<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><pre style="margin: 0; line-height: 125%"><span style="color: #0000DD; font-weight: bold">In [2]:</span> <span style="color: #008800; font-weight: bold">print</span>(student[<span style="color: red">&#39;Name&#39;</span>]) <span style="color: #888888"># displays name of the student</span><br>        <span style="color: #008800; font-weight: bold">print</span> (student<span style="color: #FF0000; color: red"></span>[<span style="color: red">&#39;class&#39;</span>]) <span style="color: #888888"># displays class of the student</span><br><br><span style="color: #fd9595; font-weight: bold">Out[2]:</span> Ernie<br>        <span>First</span></pre></div>


As seen above we have printed out the Name and Class from the dictionary. Now lets see how we can update the age from 16 to 18 and also add a new key called Address to the dictionary.

<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><pre style="margin: 0; line-height: 125%"><span style="color: #0000DD; font-weight: bold">In [2]:</span> student[<span style="color: red">&#39;Age&#39;</span>] <span style="color: #333333">=</span> <span style="color: #0000DD; font-weight: bold">18</span> <span style="color: #888888"># This updates the value for Age</span><br>        student[<span style="color: red">&#39;Address&#39;</span>] <span style="color: #333333">=</span> <span style="color: red">&#39;WestHills&#39;</span> <span style="color: #888888"># adds a new Key with the value</span></pre></div>


We have updated the Age and added the Address to our dictionary, now lets see the output.

<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><pre style="margin: 0; line-height: 125%"><span style="color: #0000DD; font-weight: bold">In [2]:</span> <span style="color: #008800; font-weight: bold">print</span>(student)<br><span style="color: #008800; font-weight: bold">        print</span>(student<span style="color: #FF0000; color: red"></span>[<span style="color: red">&#39;Age&#39;</span>])<br><span style="color: #008800; font-weight: bold">        print</span>(student[<span style="color: red">&#39;Address&#39;</span>])<br><br><span style="color: #fd9595; font-weight: bold">Out[2]:</span> {<span >&#39;Name&#39;</span>:<span>&#39;Ernie&#39;</span>,<span>&#39;Age&#39;</span>:<span>18</span>,<span>&#39;Class&#39;</span>:<span>&#39;First&#39;</span>,<span>&#39;Address&#39;</span>:<span>&#39;WestHills&#39;</span>}<br>        <span>18</span><br>        <span>WestHills</span></pre></div>


As seen above our dictionary now have the updated Age and also the new key Address

> Instructor can also inform the scholars that dictionaries can also be deleted using the Key pop() 'Age' method to delete an item in the dictionary. 
