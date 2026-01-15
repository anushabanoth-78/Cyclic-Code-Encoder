<h1>🔐 Cyclic Code Encoder (GUI-Based)</h1>

<p>
An interactive <b>GUI-based Cyclic Code Encoder</b> built using
<b>Python, Tkinter, and SymPy</b>.
</p>

<p>
This project implements <b>Cyclic Error-Correcting Codes</b> and visualizes
the complete encoding process using polynomial arithmetic over
<b>Galois Field GF(2)</b>.
</p>

<hr>

<h2>Why This Project?</h2>

<p>
Cyclic codes are a <b>fundamental concept in Digital Communication and Coding Theory</b>.
Instead of understanding them only theoretically, this project:
</p>

<ul>
  <li>Provides a practical implementation of cyclic codes</li>
  <li>Automatically computes valid generator polynomials</li>
  <li>Encodes binary messages using polynomial division</li>
  <li>Offers a simple and intuitive graphical interface</li>
</ul>

<hr>

<h2>Key Concepts Implemented</h2>

<ul>
  <li>Cyclic Codes</li>
  <li>Generator Polynomial g(x)</li>
  <li>Polynomial Arithmetic over GF(2)</li>
  <li>Error-Control Coding</li>
  <li>Linear Block Codes</li>
</ul>

<hr>

<h2>Application Walkthrough</h2>

<h3>Input Parameters</h3>

<ul>
  <li><b>n</b> – Codeword length</li>
  <li><b>k</b> – Message length</li>
  <li><b>Message Input Option</b> – Manual / Auto Generate</li>
  <li><b>Message (k bits)</b> – Binary input</li>
</ul>

<hr>

<h3>Manual Message Encoding Example</h3>

<pre>
n = 7
k = 4
Message Input Option = Manual
Message = 1011
</pre>

<p>
The application computes the generator polynomial automatically and
displays the encoded codeword.
</p>

<pre>
Generator Polynomial: x^3 + x + 1
Encoded Codeword: 1011000
</pre>

<p align="center">
  <img src="home_page_images/cyclic_code_example.png" width="500">
</p>

<hr>

<h3>Automatic Message Generation</h3>

<p>
In Auto Generate mode, the application generates a random binary message
of length <b>k</b> and encodes it using the same cyclic coding procedure.
</p>

<ul>
  <li>No manual message entry required</li>
  <li>Ensures correct binary input</li>
  <li>Useful for quick testing</li>
</ul>

<hr>

<h2>Encoding Algorithm</h2>

<ol>
  <li>Accept values of <b>n</b> and <b>k</b></li>
  <li>Compute redundancy: <b>r = n − k</b></li>
  <li>Find generator polynomial <b>g(x)</b> such that:
    <ul>
      <li>Degree of g(x) = r</li>
      <li>g(x) divides (x<sup>n</sup> − 1) over GF(2)</li>
    </ul>
  </li>
  <li>Convert message into polynomial m(x)</li>
  <li>Compute codeword:
    <br><b>c(x) = m(x) · x<sup>r</sup> + remainder</b>
  </li>
  <li>Display results in the GUI</li>
</ol>

<hr>

<h2>Features Summary</h2>

<ul>
  <li>Graphical User Interface using Tkinter</li>
  <li>Manual and automatic message input</li>
  <li>Automatic generator polynomial selection</li>
  <li>Input validation and error handling</li>
  <li>Clear display of encoded results</li>
</ul>

<hr>

<h2>Technologies Used</h2>

<ul>
  <li><b>Python 3</b></li>
  <li><b>Tkinter</b> – GUI Development</li>
  <li><b>SymPy</b> – Polynomial arithmetic over GF(2)</li>
  <li><b>Random</b> – Automatic message generation</li>
</ul>

<hr>

<h2>How to Run</h2>

<ol>
  <li>Install required package:
    <pre>pip install sympy</pre>
  </li>
  <li>Run the program:
    <pre>python cyclic_code_encoder.py</pre>
  </li>
</ol>

<p>
Ensure that <b>Python 3</b> is installed on your system.
</p>

<hr>

<h2>Input Constraints</h2>

<ul>
  <li>n must be greater than k</li>
  <li>Message length must be exactly k bits</li>
  <li>Only binary values (0 and 1) are allowed</li>
</ul>

<hr>

<h2>Learning Outcomes</h2>

<ul>
  <li>Strong understanding of cyclic codes</li>
  <li>Hands-on experience with GF(2) arithmetic</li>
  <li>GUI application development using Tkinter</li>
  <li>Applying theoretical concepts practically</li>
</ul>

<hr>

<h2>Team Project</h2>

<p>
This project was developed as a <b>group academic project</b>.
</p>

<h3>Team Members</h3>

<ul>
  <li>Pitaka Laxmi Venkata Naga Satya (2203124)</li>
  <li>Banoth Anusha (2203104)</li>
</ul>

<h3>Faculty Coordinators</h3>

<ul>
  <li>Rahul – Faculty, Computer Science</li>
  <li>Arpita – Faculty, Computer Science</li>
</ul>

<hr>

<h2>License</h2>

<p>
This project is developed for <b>academic and educational purposes only</b>.
</p>
