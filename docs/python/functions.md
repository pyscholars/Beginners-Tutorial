# Functions
A function is defined as a block of organized, reusable code used to perform a single, related action. Python has many built-in functions; you can also create your own.

Let's take a look at the print and len function in Python. 

The  **`print(object)`** function prints the given object to the standard output device (screen) or to the text stream file. That’s why if you type in **`print("Hello World")`** you get the output `Hello World`. 

Same goes for len, The **`len(object)`** function returns the number of items in an object.When the object is a string, the **`len()`** function returns the number of characters in the string.

Now let's create our own function to use for greeting.

<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><pre style="margin: 0; line-height: 125%"><span style="color: #0000DD; font-weight: bold">In [2]:</span> <span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">greet</span> (name):<br>        <span style="color: #DD4422">&quot;&quot;&quot;This function greets</span><br><span style="color: #DD4422">         the name passed in as</span><br><span style="color: #DD4422">         parameter&quot;&quot;&quot;</span><br>         <span style="color: #008800; font-weight: bold">print</span>(<span style="color: red">&quot;Good morning! Mr &quot;</span><span style="color: #333333">+</span> name <span style="color: #333333">+</span><span style="color: red">&quot;. How are you doing today? &quot;</span>)</pre></div>



So above we have defined our function greet, lets see what happens when we execute our function.

<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><pre style="margin: 0; line-height: 125%"><span style="color: #0000DD; font-weight: bold">In [2]:</span> greet(<span style="color: red">&#39;Michael&#39;</span>)<br><br><span style="color: #fd9595; font-weight: bold">Out[2]:</span> Good morning<span>!</span> Mr Michael<span style="color: #333333">.</span> How are you doing today<span>?</span></pre></div>


So we can see that when we made the object name **"Michael"** we have an output that greets Michael from the function. Now the advantage of this is let’s assume you have an app that need to greet a user. To do that in your application, you just call on the function greet to handle that.

