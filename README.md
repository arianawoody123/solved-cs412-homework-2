Download Link: https://assignmentchef.com/product/solved-cs412-homework-2
<br>



<ul>

 <li>Feel free to talk to other members of the class when doing the homework. We are more concerned that you learn how to solve the problem than that you demonstrate that you solved it entirely on your own. You should, however, write down your solution yourself. Please try to keep the solution brief and clear.</li>

 <li>Please use Piazza first if you have questions about the homework. Also feel free to send us e-mails and come to office hours.</li>

 <li>The homework is due at 11:59 PM on the due date. We will be using Compass (http: //compass2g.illinois.edu) for collecting homework assignments. Please do NOT hand in a hard copy of your write-up. Contact the TAs if you are having technical difficulties in submitting the assignment. We do NOT accept late homework!</li>

 <li>The homework should be submitted in pdf format. If you use additional source code for solving problems, you are required to submit them and use the file names to identify the corresponding questions. For instance, ‘Problem1.netid.py’ refers to the python source code for Problem 1, replace netid with your netid. Compress all the files (pdf and source code files) into one zip file. Submit the compressed file ONLY. (If you did not use any source code, submitting the pdf file without compression will be fine)</li>

 <li>For each question, you will NOT get full credit if you only give out a final result. Necessary calculation steps are required. If the result is not an integer, round your result to 3 decimal places.</li>

</ul>

<strong>Problem 1.</strong>

Suppose the base cuboid of a data cube contains two cells:

(<em>a</em><sub>1</sub><em>,a</em><sub>2</sub><em>,a</em><sub>3</sub><em>,a</em><sub>4</sub><em>,a</em><sub>5</sub><em>,a</em><sub>6</sub><em>,a</em><sub>7</sub><em>,a</em><sub>8</sub><em>,a</em><sub>9</sub><em>,a</em><sub>10</sub>) : 1<em>,</em>(<em>a</em><u><sub>1</sub></u><em>,b</em><sub>2</sub><em>,a</em><u><sub>3</sub></u><em>,b</em><sub>4</sub><em>,b</em><sub>5</sub><em>,b</em><sub>6</sub><em>,b</em><sub>7</sub><em>,b</em><sub>8</sub><em>,a</em><u><sub>9</sub></u><em>,b</em><sub>10</sub>) : 1 where <em>a<sub>i </sub></em>6= <em>b<sub>i </sub></em>for any <em>i</em>.

<ul>

 <li>(3 points) How many cuboids are there in this data cube?</li>

 <li>(5 points) How many (nonempty) closed cells are there in this data cube?</li>

 <li>(5 points) How many (nonempty) aggregate cells are there in this data cube?</li>

 <li>(5 points) How many (nonempty) aggregate closed cells are there in this data cube?</li>

 <li>(5 points) If we set minimum support = 2, how many (nonempty) aggregate cells arethere in the corresponding iceberg cube?</li>

</ul>

<strong>Problem 2. </strong>

We have the following data cube measures. Which of them are algebraic measures? Explain each of your selection and non-selection.

<ul>

 <li>(5 points) Standard deviation;</li>

 <li>(5 points) Average of Min and Max;</li>

 <li>(5 points) Sum of the largest 50 values;</li>

 <li>(5 points) Sum of the largest values, where <em>n </em>is the number of data points in the current <strong>cuboid </strong>and b<em>x</em>c denotes the greatest integer less than or equal to <em>x</em>; (e) (5 points) Mode, if the data is guaranteed to be binary.</li>

</ul>

<strong>Problem 3. </strong>

A database has 5 transactions listed in Table 1. Let <em>min sup </em>= 0<em>.</em>6 and <em>min conf </em>= 0<em>.</em>7.

Table 1:

<table width="197">

 <tbody>

  <tr>

   <td width="69">trans id</td>

   <td width="128">item bought</td>

  </tr>

  <tr>

   <td width="69">001</td>

   <td width="128">{H, A, D, B, C}</td>

  </tr>

  <tr>

   <td width="69">002</td>

   <td width="128">{D, A, E, F}</td>

  </tr>

  <tr>

   <td width="69">003</td>

   <td width="128">{C, D, B, E}</td>

  </tr>

  <tr>

   <td width="69">004</td>

   <td width="128">{B, A, C, H, D}</td>

  </tr>

  <tr>

   <td width="69">005</td>

   <td width="128">{B, G, C}</td>

  </tr>

 </tbody>

</table>

<ul>

 <li>(5 points) List the frequent <em>k</em>-itemset for the largest <em>k</em>;</li>

 <li>(3 points) Show an itemset <em>S</em>, where (1) ∀<em>S</em><sub>0 </sub>⊂ <em>S </em>(<em>S</em><sub>0 </sub>6= ∅), <em>S</em><sub>0 </sub>is frequent, and (2) <em>S </em>is not frequent;</li>

 <li>(5 points) List all the closed patterns;</li>

 <li>(5 points) List all the max-patterns;</li>

 <li>(5 points) List all the strong association rules (with support and confidence) with thefollowing shape: <em>x </em>∈{001<em>,</em>002<em>,…,</em>005}<em>, buys</em>(<em>x,item</em><sub>1</sub>) ∧ <em>buys</em>(<em>x,item</em><sub>2</sub>) ⇒ <em>buys</em>(<em>x,item</em><sub>3</sub>). [<em>s,c</em>].</li>

 <li>(5 points) Now we want to mine frequent patterns using FP-Growth. We first find singleitem frequent patterns and sort them in frequency descending order. To break ties, we assume the order is <em>B </em>− <em>C </em>− <em>D </em>− <em>A</em>. Construct the FP-tree;</li>

 <li>(5 points) Show <em>A</em>’s conditional (i.e., projected) database.</li>

</ul>

<strong>Problem 4. </strong>

Suppose we are interested in only the frequent patterns satisfying certain constraints. For example, in Table 1, each item has its price. The price information is listed in Table 2. We still have <em>min sup </em>= 0<em>.</em>6.

Table 2:

<table width="301">

 <tbody>

  <tr>

   <td width="49">item</td>

   <td width="40">A</td>

   <td width="31">B</td>

   <td width="32">C</td>

   <td width="32">D</td>

   <td width="32">E</td>

   <td width="32">F</td>

   <td width="32">G</td>

   <td width="24">H</td>

  </tr>

  <tr>

   <td width="49">price</td>

   <td width="40">10</td>

   <td width="31">20</td>

   <td width="32">40</td>

   <td width="32">30</td>

   <td width="32">90</td>

   <td width="32">90</td>

   <td width="32">30</td>

   <td width="24">50</td>

  </tr>

 </tbody>

</table>

<ul>

 <li>(5 points) Find all the <em>frequent </em>patterns <em>S </em>in Table 1 satisfying <em>sum</em>(<em>price</em>) ≥ 45 (i.e.,</li>

</ul>

the sum of the price of all the items in <em>S </em>is no less than 45);

<ul>

 <li>(8 points) Is the constraint <em>sum</em>(<em>price</em>) ≥ 45 monotonic or anti-monotonic? How about <em>sum</em>(<em>S.price</em>) ≤ 45? Can you find an efficient method to mine <em>frequent </em>patterns with</li>

</ul>

<em>sum</em>(<em>S.price</em>) ≤ 45?

<ul>

 <li>(6 points) Let us focus on two other constraints <em>avg</em>(<em>price</em>) ≥ 30 (i.e., the average price of all the items in <em>S </em>is no less than 30) and <em>avg</em>(<em>S.price</em>) ≤ 30. Are they convertible? If so, how to convert them to anti-monotonic cases?</li>

</ul>