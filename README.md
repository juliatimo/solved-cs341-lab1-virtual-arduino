Download Link: https://assignmentchef.com/product/solved-cs341-lab1-virtual-arduino
<br>
The goal in this lab will be get familiar with a program that mimics an Arduino Uno.

<h1>Making an Account and getting started</h1>

The website we will be using is <a href="https://www.tinkercad.com/">https://www.tinkercad.com</a><a href="https://www.tinkercad.com/">.</a> There is the functionality to have a class on tinkercad, but we won’t be using that feature this semester.

<ol>

 <li>Click “join now” and create a personal account (this is free)</li>

 <li>Click the logo in the top left corner to get to your main page</li>

 <li>Click “Circuits” and then “create new Circuit”</li>

 <li>Here you’ll see the Arduino simulator</li>

</ol>

<h1>Creating your first circuit</h1>

In this lab we will do a simple circuit to get you familiar with Arduino. We will blink a led and say “hello world!”

<ol>

 <li>Use the components window on the far right to get a breadboard and an Arduino Uno. Drag and drop into the middle of the screen</li>

</ol>




The breadboard will be used for connecting wires. It is less useful when wiring digitally and in the future you may decide to wire components directly together. However, for lab 1 I am requiring you to use the breadboard in case you ever need to use one in real life.

If you move your mouse around the breadboard you will see holes light up green. This is to show what holes are connected underneath the breadboard. For instance, 12a through 12e are all connected to one another.

<ol start="2">

 <li>Make the connections (pin 13 -&gt; b2) and (b1 -&gt; GND)</li>

 <li>Grab a led from the components and connect it to j1 and j2</li>

 <li>Connect a resistor to d2 and f2</li>

 <li>Lastly finish the circuit by connecting (e1 -&gt; f1)</li>

</ol>

<h1>Coding in Arduino</h1>

Now we need to write some code. First, we need to tell the Arduino to blink pin 13 (which our led is connected to). Second, we need to print “hello world”.

<ol>

 <li>Click the “code” button in the top right</li>

 <li>Switch from “blocks” to “text”</li>

</ol>

Side Note: do not use blocks coding as it is meant for middle-school children.

<ol start="3">

 <li>You should see the default code:</li>

</ol>




First, you may notice that the notation looks familiar. Arduino is technically its own language, but it is a part of the C and C++ family. One distinct difference is the use of setup() and loop(). Setup() will be ran once at the beginning of execution, and loop() will run continuously after setup().




<ol start="4">

 <li>Click “Start Simulation” and your LED should blink</li>

 <li>Now add the two following lines to setup():</li>

</ol>

Serial.begin(9600);

Serial.print(“Hello, World!”);

<ol start="6">

 <li>Rerun the code and click “Serial Monitor” at the bottom right of your screen</li>

</ol>

<h1>Some Extra Things to Explore</h1>

<ol>

 <li>Try to change how long the led blinks for.</li>

 <li>Try changing the amount of resistance on the resistor. What happens?</li>

 <li>Try rotating the led 180 degrees. You can do this by clicking on it and clicking the rotate button in the top left corner. Now the longer lead (anode) should be in j1, and the shorter lead (cathode) should be in j2.</li>

</ol>