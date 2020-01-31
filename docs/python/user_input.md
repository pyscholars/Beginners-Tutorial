# User Input

Python has an input function which allows a user enters an input. You call this function to tell the program to stop and wait for the user to key in the data. The program will resume once the user presses the **ENTER** or **RETURN** key.

<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><pre style="margin: 0; line-height: 125%"><span style="color: #0000DD; font-weight: bold">In [2]:</span> name <span style="color: #333333">=</span> <span style="color: #007020">input</span>(<span style="color: red">&quot;What is your name: &quot;</span>)</pre></div>


Above we have created a variable to request the name of our user. Lets see what the output would be.

<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><pre style="margin: 0; line-height: 125%"><span style="color: #0000DD; font-weight: bold">In [2]:</span> name <span style="color: #333333">=</span> <span style="color: #007020">input</span>(<span style="color: red">&quot;What is your name: &quot;</span>)<br>        <span style="color: #008800; font-weight: bold">print</span>(<span style="color: red">&quot;Did you say your name is?&quot;</span>, name)<br><br><span style="color: #fd9595; font-weight: bold">Out[2]:</span> What is your name: <input type="text" disabled></pre></div>

Now the program is waiting for the user’s input. We have added an output to ask the user if the name they provided was okay.

<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><pre style="margin: 0; line-height: 125%"><span style="color: #0000DD; font-weight: bold">In [2]:</span> name <span style="color: #333333">=</span> <span style="color: #007020">input</span> (<span style="color: red">&quot;What is your name: &quot;</span>)<br>        <span style="color: #008800; font-weight: bold">print</span> (<span style="color: red">&quot;Did you say your name is?&quot;</span>, name)<br><br><span style="color: #fd9595; font-weight: bold">Out[2]:</span> What <span>is</span> your name: Mannie Young<br>        <span>Did you say your name is<span>?</span> Mannie Young</span></pre></div>


Above we can see that the user gave an input **Mannie Young** which was stored and asked if the name was correct. 

Lets try and asked for the user’s favorite number.

<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><pre style="margin: 0; line-height: 125%"><span style="color: #0000DD; font-weight: bold">In [2]:</span> favNum <span style="color: #333333">=</span> <span style="color: #007020">input</span> (<span style="color: red">&quot;Whats&#39;s your favorite number: &quot;</span>)<br>        <span style="color: #008800; font-weight: bold">print</span> (<span style="color: red">&quot;</span><span style="color: #666666; font-weight: bold; color: red">\n</span><span style="color: red"> Your favorite number is: &quot;</span>, favNum)<br><br><span style="color: #fd9595; font-weight: bold">Out[2]:</span> What<span>&#39;s your favorite number: <input type="text" value="7" disabled></span><br>        <span>Your favorite number is: 7</span></pre></div>


Above we can see that the input was 7. We would notice that for the first time we have a line break between the question and the output, this was made possible by the \n which means new line.  