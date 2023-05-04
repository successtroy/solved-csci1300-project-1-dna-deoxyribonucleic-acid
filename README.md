Download Link: https://assignmentchef.com/product/solved-csci1300-project-1-dna-deoxyribonucleic-acid
<br>
<h1>Objectives</h1>

<ul>

 <li>Understand and work with functions and strings</li>

 <li>Be able to test functions</li>

</ul>

You can find <a href="https://moodle.cs.colorado.edu/pluginfile.php/212362/mod_folder/content/0/project1_background.pdf?forcedownload=1"><strong>project1 note: functions and string</strong></a>​ <a href="https://moodle.cs.colorado.edu/pluginfile.php/212362/mod_folder/content/0/project1_background.pdf?forcedownload=1"><strong>s</strong></a> <u>​ </u>on Moodle.

<h2>Question 1: pyramid, surface area</h2>

A Pyramid with a square base, 4 triangular faces, and an apex is a square pyramid. Write a function ​ <strong>surfaceArea</strong>​               ​ to calculate and return​             the surface area of a square pyramid. The function takes <strong>two double</strong>​         <strong> parameters</strong> – the base length(b) and slant height(s) of a square​      pyramid, and calculates and returns the surface area as a <strong>double</strong>​                .​

<em>Function specifications:  </em>

<ul>

 <li>The function name: <strong>surfaceArea</strong>​</li>

 <li>The function parameters (in this order)</li>

</ul>

○    The base length, double​

○    The slant height, double​

<ul>

 <li>The function return value: surface area, double​           The function should not print anything.</li>

 <li>Edge cases: if one or more arguments are not positive numbers, then it should return -1</li>

</ul>




Sample run 1 (<strong>bold</strong>​ is user input)​

Enter the base length: <strong>3</strong>​

Enter the slant height: <strong>4</strong>​

The surface area: 33




Sample run 2 (<strong>bold</strong>​ is user input)​

Enter the base length: <strong>3</strong>​

Enter the slant height: <strong>-1</strong>​

Invalid values




The file should be named as pyramid.cpp​ . Don’t forget to head over to the code runner on​        Moodle and paste only your function in the answer box! In the main, make sure that you call the function and output the surface area.

<h2>Question 2: Braking Distance</h2>

Displacement, D (i.e. a distance) for a braking vehicle can be calculated with the initial velocity, <strong>I</strong>​, the final velocity, ​<strong>F</strong>​, and deceleration,​<strong> a</strong>​.

Write a function called ​<strong>displacement</strong>​ that takes as parameters: initial velocity, ​<strong>I</strong>​, final velocity <strong>F</strong>​, and deceleration​ ​<strong>a</strong>​<strong>. </strong>

Function specifications: <strong> </strong>

<ul>

 <li>Your function must be named ​<strong>displacement </strong></li>

 <li>Your function takes three parameters (all double, in this order)</li>

</ul>

○    Initial velocity ​<strong>I</strong>

○    Final velocity ​<strong>F</strong>

○    Deceleration ​<strong>a</strong>

<ul>

 <li>Your function should return the appropriate displacement, ​<strong>D</strong>​, of the vehicle as ​double​. If one or more values are invalid, the function print all the error messages in this order and return ​0​.</li>

 <li>If your function receives negative velocities then it must print “​Velocity should be greater than zero.​”</li>

 <li>If your function receives a zero deceleration then it must print “​No brakes were applied.​”</li>

 <li>If your function receives a negative deceleration then it must print “​The vehicle is speeding up.​”</li>

 <li>If your function receives ​<strong>F &gt; I</strong>​ then it must print “​Error in acceleration values.​”</li>

</ul>




<strong>For example:</strong>​ Bob is riding his bicycle to the store at a velocity of 4 m/s, when an aardvark runs out in front of him. He quickly brakes to a complete stop, with a deceleration of 2 m/s. What is his displacement?

Note that because Bob is stopped, the final velocity, ​F = 0​. His initial velocity, ​I = 4​ m/s. The deceleration is ​2​ m/s.

Therefore the function should return 4.

Sample run 1 (<strong>bold</strong>​ is user input)​

Enter initial velocity: <strong>10</strong>​

Enter final velocity: <strong>1</strong>​

Enter deceleration: <strong>5</strong>​

Displacement is 9.9

Sample run 2 (<strong>bold</strong>​ is user input)​

Enter initial velocity: <strong>1</strong>​

Enter final velocity: <strong>2</strong>​ Enter deceleration: <strong>0</strong>​

No brakes were applied.

Error in acceleration values.

The file should be named as displacement.cpp​  . Don’t forget to head over to the code​              runner on Moodle and paste only your function in the answer box! In the main, make sure that you call the function and output the displacement.

<h2>Question 3: change to upper case</h2>

Write a function called <strong>toUpper</strong>​          that has a single parameter and returns a new string with all​              characters converted to uppercase.




<em>Function specifications</em>​:

<ul>

 <li>The function name: <strong>toUpper</strong>​          The function parameter</li>

</ul>

○    The string that will be converted to upper cases, string​     ●      The function return value: the string with all upper cases, string​  ●      The function should not print anything.

<ul>

 <li>Edge cases: Non alphabetical characters remain unchanged.</li>

</ul>




Sample run 1 (<strong>bold</strong>​ is user input)​

Enter the string:          <strong>Convert this string to UPPER case!!!</strong>​      CONVERT THIS STRING TO UPPER CASE!!!




The file should be named as toUpper.cpp​ . Don’t forget to head over to the code runner on​        Moodle and paste only your function in the answer box! In the main, make sure that you call the function and output the surface area.

<h1>DNA Analyzer</h1>

<h2>Background: Measuring DNA Similarity</h2>

<strong> </strong>

<a href="https://en.wikipedia.org/wiki/DNA">DNA</a> <u>​ </u>is the hereditary material in humans and other species. Almost every cell in a person’s body has the same DNA. All information in DNA is stored as code in four chemical bases: adenine (<strong>A</strong>​ )​ , guanine (<strong>G</strong>​ )​ , cytosine (<strong>C</strong>​ )​ and thymine (<strong>T</strong>​ )​ .  The differences in the order of these bases is a means of specifying different information.




We refer to an organism’s complete set of chemical bases as their <em>genome</em>​               ​. Every genome looks something like this:




GATCAATGAGGTGGACACCAGAGGCGGGGACTTGTAAATAACACTGGGCTGTAGGAGTGATGGGGTTCACCTCTAATTCTAAGATGGCTAGATAAT

GCATCTTTCAGGGTTGTGCTTCTATCTAGAAGGTAGAGCTGTGGTCGTTCAATAAAAGTCCTCAAGAGGTTGGTTAATACGCATGTTTAATAGTACA GTATGGTGACTATAGTCAACAATAATTTATTGTACATTTTTAAATAGCTAGAAGAAAAGCATTGGGAAGTTTCCAACATGAAGAAAAGATAAATGGTC

AAGGGAATGGATATCCTAATTACCCTGATTTGATCATTATGCATTATATACATGAATCAAAATATCACACATACCTTCAAACTATGTACAAATATTATAT

ACCAATAAAAAATCATCATCATCATCTCCATCATCACCACCCTCCTCCTCATCACCACCAGCATCACCACCATCATCACCACCACCATCATCACCAC

CACCACTGCCATCATCATCACCACCACTGTGCCATCATCATCACCACCACTGTCATTATCACCACCACCATCATCACCAACACCACTGCCATCGTCA

TCACCACCACTGTCATTATCACCACCACCATCACCAACATCACCACCACCATTATCACCACCATCAACACCACCACCCCCATCATCATCATCACTAC

TACCATCATTACCAGCACCACCACCACTATCACCACCACCACCACAATCACCATCACCACTATCATCAACATCATCACTACCACCATCACCAACACC

A

<a href="http://www.sacred-texts.com/dna/hgp011k.htm">Human Genome: First 1000 lines of Chromosome 1</a>

The human genome has about 3 billion DNA base pairs. That means the entire human genome can be represented by a (very long) string of ~3 billion characters, where every character in the string is A, C, G, or T. You can find the first 1000 lines of Chromosome 1 of the Human Genome at <a href="http://www.sacred-texts.com/dna/hgp011k.htm">this webpag</a><u>​     </u><a href="http://www.sacred-texts.com/dna/hgp011k.htm">e</a><a href="http://www.sacred-texts.com/dna/hgp011k.htm">.</a><u>​</u>

In the lectures, there have been examples of string representation and use in C++. In this assignment, we will create strings that represent DNA sequences.  We will be implementing a number of functions that are used to search for substrings that represent sequences within the DNA.

Interaction of DNA (orange) with histones (blue), a DNA binding protein. These proteins’ basic amino acids bind to the acidic phosphate groups on DNA. <a href="https://commons.wikimedia.org/wiki/User:Splette">Thomas Splettstoesser</a>

One of the challenges in <a href="https://en.wikipedia.org/wiki/Computational_biology">computational biolog</a><u>​              </u><a href="https://en.wikipedia.org/wiki/Computational_biology">y</a><u>​</u> is determining where a <a href="https://en.wikipedia.org/wiki/DNA-binding_protein">DNA binding protei</a>​ <a href="https://en.wikipedia.org/wiki/DNA-binding_protein">n</a> <u>​ </u>will bind in a genome.  Each DNA binding protein has a preference for a specific sequence of nucleotides.  This preference sequence is known as a motif.  The locations of a motif within a genome are important to understanding the behavior of a cell’s response to a changing environment.

To find each possible location along the DNA, we must consider how well the motif matches the DNA sequence at each possible position.  The protein does not require an exact match to bind and can bind when the sequence is similar to the motif.

Another common DNA analysis function is the comparison of newly discovered DNA genomic sequences to the large databases of known DNA sequences and using the similarity of the sequences to help identify the origin of the new sequences.




<h2>Goal of your project</h2>

Suppose that the emergency room of a hospital sees a sudden and drastic increase in patients presenting with a particular set of symptoms. Doctors determine the cause to be bacterial, but without knowing the specific species involved they are unable to treat patients effectively. One way of identifying the cause is to obtain a DNA sample and compare it against known bacterial genomes. With a set of similarity scores, doctors can make more informed decisions regarding treatment, prevention, and tracking of the disease.




For this project (questions 4 – 7) you will be writing a program that performs three main functionalities:

<ul>

 <li>Calculate the similarity score (This will be question 4)</li>

 <li>Find the best similarity score in the given genome (This will be question 5)</li>

 <li>Given three genomes and a sequence from the unknown bacteria, determine the most probable match (This will be question 6)</li>

</ul>




So, in question 7, you will be developing the main​    function using the functions you create in​      problems 4-6. We’ve nicely broken down this program into three functions. You’re welcome to write additional helper functions as you need. Write your code and test each function on your Cloud 9. Then, once you complete, you can submit it on Moodle coderunner to make sure it’s fully functional. All the functions and the main​ function should be in one file,​

DNAanalyzer.cpp.​




<h3>Question 4: calcSimScore</h3>

Write a function <strong>calcSimScore</strong>​         that returns the similarity score for two sequences. The​        similarity score for two sequences is calculated as follows:

similarity_score = (string_length – hamming_distance) / string_length

Where <a href="https://en.wikipedia.org/wiki/Hamming_distance">hamming distanc</a><u>​            </u><a href="https://en.wikipedia.org/wiki/Hamming_distance">e</a> is the number of positions at which the corresponding characters are​        different. Two strings with a small Hamming distance are more similar than two strings with a larger Hamming distance. <u>The two strings must always be the same length</u><u>​             </u> when calculating a<u>​       </u> Hamming distance. If the length of the genomes is different, then the similarity score cannot be calculated. Similarity score will be in the range [0.0,1.0].




<strong>Example</strong>:​           first string = “ACCT”               second string = “ACCG”




A  C C T

|   |   |  *

A C C G

In this example, string_length = 4. Since there is one mismatch, the hamming_distance = 1 . And the similarity score for the two strings on this example would be, similarity_score = (4-1)/4 =  3/4   = 0.75

<em>Function specifications</em>​:

<ul>

 <li>The function name: <strong>calcSimScore</strong>​</li>

 <li>The function parametesr(in this order):</li>

</ul>

○    Sequence 1, string​

○    Sequence 2, string​

<ul>

 <li>The function should return the similarity score as a double​</li>

 <li>If the length of the strings is the same, then the function calculates the similarity score. If not, the similarity score would be 0.</li>

 <li>The function should not print anything.</li>

</ul>




<strong>Examples: </strong>Arguments and their expected return values for the ​ calcSimScore​

<table width="624">

 <tbody>

  <tr>

   <td width="208"><strong>sequence1 </strong></td>

   <td width="208"><strong>sequence2 </strong></td>

   <td width="208"><strong>Similarity score  </strong></td>

  </tr>

  <tr>

   <td width="208">ATGC</td>

   <td width="208">ATGA</td>

   <td width="208">0.75</td>

  </tr>

  <tr>

   <td width="208">CCDCCD</td>

   <td width="208">CCDCCD</td>

   <td width="208">1</td>

  </tr>

  <tr>

   <td width="208">ATG</td>

   <td width="208">GAT</td>

   <td width="208">0</td>

  </tr>

  <tr>

   <td width="208">ACCDT</td>

   <td width="208">ACT</td>

   <td width="208">0</td>

  </tr>

 </tbody>

</table>




Once you have tested your code on Cloud 9 / VS code, then head over to code runner on Moodle and only your function in the answer box! Make sure that your unit tests are in the main function (commented out).

<h3>Question 5: findBestSimScore</h3>

Write a function called <strong>findBestSimScore</strong>​ that takes a genome and a sequence and returns​     the highest similarity score found in the genome as a double.

Note: the term genome refers to the string that represents the complete set of genes in an organism, and sequence to refer to some substring or sub-sequence in the genome.

<em>Function specifications</em>​:

<ul>

 <li>The function name: <strong>findBestSimScore</strong>​          The function parameters(in this order):</li>

</ul>

○    a string parameter for the genome (complete set of genes) ○          a string parameter for the sequence (sub-sequence of the genome)  ●  The function should return the highest similarity score as a double.

<ul>

 <li>If the length of the sequence is longer than the genome, then the function should return</li>

</ul>

<ol>

 <li>(the best similarity score is 0)</li>

</ol>

<ul>

 <li>The function should not print anything.</li>

 <li>The best similarity scores is [0.0,1.0]</li>

</ul>

<strong>Note</strong>:​ Our sequence is “ACT”, which is a string of length 3. That means we need to compare our sequence with all the 3 character long sub-sequences (substrings) in the genome. Follow the example below:

<table width="343">

 <tbody>

  <tr>

   <td width="115">genome sub-sequence</td>

   <td width="84">sequence</td>

   <td width="144">similarity score</td>

  </tr>

  <tr>

   <td width="115"><strong>ATA</strong>​CGC</td>

   <td width="84"><strong>ACT </strong></td>

   <td width="144">0.33</td>

  </tr>

  <tr>

   <td width="115">A​<strong>TAC</strong>​GC</td>

   <td width="84"><strong>ACT </strong></td>

   <td width="144">0</td>

  </tr>

  <tr>

   <td width="115">AT​<strong>ACG</strong>​C</td>

   <td width="84"><strong>ACT </strong></td>

   <td width="144">0.66</td>

  </tr>

  <tr>

   <td width="115">ATA​<strong>CGC </strong></td>

   <td width="84"><strong>ACT </strong></td>

   <td width="144">0</td>

  </tr>

 </tbody>

</table>




←  <strong>findBestSimScore </strong>​             returns 0.66,​     since that is the highest similarity score found

Once you have tested your code on Cloud 9 / VS code,  then head over to code runner on Moodle and only your functions in the answer box! Make sure that your unit tests are in the main function (commented out).

<h3>Question 6: findMatchedGenome</h3>

Write a function called findMatchedGenome that takes three genomes and a sequence and prints the list of matched genomes.

<em>Function specifications</em>​:

<ul>

 <li>The function name: <strong>findMatchedGenome</strong>​          The function parameters(in this order):

  <ul>

   <li>Genome 1, a string</li>

  </ul></li>

</ul>

○    Genome 2, a string

○    Genome 3, a string

○    sequence (sub-sequence of the genomes), a string  ●         The function should not return anything.

<ul>

 <li>Unexpected values might be passed into the function and your function should be able to handle them without crashing the program:

  <ul>

   <li>Case 1: If one or more genomes or the sequence is an empty string, then your function should <strong>only</strong>​ print  “​ Genomes or sequence is empty.​           ”​</li>

  </ul></li>

</ul>

○ Case 2: If the length of the three genomes are different, your function should only print  “Lengths of genomes are different.​             ”​

○    Your function must check these cases in the order specified above; i.e. first check for empty genomes or sequences, then check for different length genomes.




We compute the highest similarity scores found in each genome. Among the three highest similarity scores, the best matched genome is the one with the highest similarity score. If two or more genomes have the same highest similarity scores, then it lists the genomes with the highest similarity score.




<table width="624">

 <tbody>

  <tr>

   <td width="123">genome 1</td>

   <td width="501">AATGTTTCAC</td>

  </tr>

  <tr>

   <td width="123">genome 2</td>

   <td width="501">GACCGACTAA</td>

  </tr>

  <tr>

   <td width="123">genome 3</td>

   <td width="501">AAGGTGCTCC</td>

  </tr>

  <tr>

   <td width="123">sequence</td>

   <td width="501">TACTA</td>

  </tr>

  <tr>

   <td colspan="2" width="624">Genome 2 is the best match.</td>

  </tr>

 </tbody>

</table>

<strong>Example1:</strong> One of the genomes has the best match​




<em>Explanation:</em>

Since the length of the three genomes (genome1, genome2 and genome3) are the same, we calculate the best similarity score with each genome. The best-matched genome is then calculated based on the highest of the previously calculated best similarity scores.

<strong> </strong>

<strong> </strong>

<table width="624">

 <tbody>

  <tr>

   <td width="96"> </td>

   <td width="250"> </td>

   <td width="278">Highest similarity score</td>

  </tr>

  <tr>

   <td width="96">genome 1</td>

   <td width="250">AATGT​<strong>TTCAC </strong></td>

   <td width="278">0.4</td>

  </tr>

  <tr>

   <td width="96">genome 2</td>

   <td width="250">GACC​<strong>GACTA</strong>​A</td>

   <td width="278">0.8</td>

  </tr>

  <tr>

   <td width="96">genome 3</td>

   <td width="250">AAGG​<strong>TGCTC</strong>​C</td>

   <td width="278">0.6</td>

  </tr>

 </tbody>

</table>




The best similarity score for genome1 and sequence is 0.4, for genome2 and sequence is 0.8, and for genome3 and sequence is 0.6. Since genome 2 has the highest similarity scores among the three genomes, genome 2 is best matched.




<table width="624">

 <tbody>

  <tr>

   <td width="123">genome 1</td>

   <td width="501">AACT</td>

  </tr>

  <tr>

   <td width="123">genome 2</td>

   <td width="501">AACT</td>

  </tr>

  <tr>

   <td width="123">genome 3</td>

   <td width="501">AATG</td>

  </tr>

  <tr>

   <td width="123">sequence</td>

   <td width="501">AACT</td>

  </tr>

  <tr>

   <td colspan="2" width="624">Genome 1 is the best match. Genome 2 is the best match.</td>

  </tr>

 </tbody>

</table>

<strong>Example2:</strong> Two genomes match with a sequence​




<em>Explanation:  </em>

The best-matched genome is calculated based on the highest similarity scores given in each sequence.

<table width="624">

 <tbody>

  <tr>

   <td width="173"> </td>

   <td width="247"><strong> </strong></td>

   <td width="204"><strong>Highest Similarity Score </strong></td>

  </tr>

  <tr>

   <td width="173">genome 1</td>

   <td width="247"><strong>AACT </strong></td>

   <td width="204">1.0</td>

  </tr>

  <tr>

   <td width="173">genome 2</td>

   <td width="247"><strong>AACT </strong></td>

   <td width="204">1.0</td>

  </tr>

  <tr>

   <td width="173">genome 3</td>

   <td width="247">AATG</td>

   <td width="204">0.5</td>

  </tr>

 </tbody>

</table>

<em> </em>

The length of the three genomes are the same, so we calculate the best similarity score. The best similarity for genome1 and genome2 will be 1.0, while the genome3 is 0.5. Since genome 1 and 2 have higher similarity scores than the genome3, it will be printed in the format specified.




<strong>Example 3 (edge case)</strong>:​ length of genomes is different <strong> </strong>

<table width="624">

 <tbody>

  <tr>

   <td width="123">genome 1</td>

   <td width="501">AACTC</td>

  </tr>

  <tr>

   <td width="123">genome 2</td>

   <td width="501">AACT</td>

  </tr>

  <tr>

   <td width="123">genome 3</td>

   <td width="501">AATG</td>

  </tr>

  <tr>

   <td width="123">sequence</td>

   <td width="501">AACT</td>

  </tr>

  <tr>

   <td colspan="2" width="624">Lengths of genomes are different.</td>

  </tr>

 </tbody>

</table>




<strong>Example 4 (edge case):</strong> One or more genomes or sequence is empty​

<table width="624">

 <tbody>

  <tr>

   <td width="123">genome 1</td>

   <td width="501">AACTC</td>

  </tr>

  <tr>

   <td width="123">genome 2</td>

   <td width="501"> </td>

  </tr>

  <tr>

   <td width="123">genome 3</td>

   <td width="501">AATG</td>

  </tr>

  <tr>

   <td width="123">sequence</td>

   <td width="501">AACT</td>

  </tr>

  <tr>

   <td colspan="2" width="624">Genomes or sequence is empty.</td>

  </tr>

 </tbody>

</table>




Once you have tested your code on Cloud 9 / VS code, then head over to code runner on Moodle and paste only your functions in the answer box! Make sure that your unit tests are in the main function (commented out).




<h3>Question 7: Put it all together</h3>

To make it usable for doctors and researchers, we’ll create a menu option and call the appropriate functions you have created.




The menu has the following options:

<ol>

 <li>Calculate similarity score</li>

 <li>Find the best similarity score</li>

 <li>Analyze the genome sequences</li>

 <li>Quit</li>

</ol>




The menu will run on a loop, continually offering the user four options until they opt to quit. You need to fill in the code for each of the options. Be sure to use the functions you wrote in questions 4-6.

<strong>Option1</strong>:​ Find similarity score

The program asks two sequences (sequence1 and sequence2), then it displays the similarity score between the two sequences.

Enter sequence 1: <strong>AACT </strong>

Enter sequence 2:

<strong>AATC </strong>

Similarity score: 0.5







<strong>Option2</strong>:​ Find the best similarity score

The program asks for a genome and sequence (subset of the genome) and it displays the highest similarity scores found in the genome.

<table width="624">

 <tbody>

  <tr>

   <td width="624">Enter genome:<strong>AATCTCTTTAA </strong>Enter sequence:<strong>TCA </strong>Best similarity score: 0.666667</td>

  </tr>

 </tbody>

</table>




<strong>Option3</strong>:​ Analyze the genome sequences

In this option, the program takes 3 genomes and a sequence and shows the best matched genome.

Enter genome 1: <strong>AATGTTTCAC </strong>Enter genome 2: <strong>GACCGACTAA </strong>Enter genome 3: <strong>AAGGTGCTCC </strong>Enter sequence:

<strong>TACTA </strong>

Genome 2 is the best match.




<strong>Option4</strong>:​ Quit

When the user opt this option, the program prints “Good bye!”​ And exits the program.​




<h3>Invalid option</h3>

Your program should be able to handle the user error (i.e. users might choose the option that is not listed). If an invalid option is entered, the program should display “Invalid​             option.” and show the menu options again.




Sample run (<strong>bold</strong>​ is user input)​

Select a numerical option:

=== menu ===

<ol>

 <li>Find similarity score</li>

 <li>Find the best similarity score</li>

 <li>Analyze the genome sequences</li>

 <li>Quit</li>

</ol>

<strong>10 </strong>

Invalid option.

Select a numerical option:

=== menu ===

<ol>

 <li>Find similarity score</li>

 <li>Find the best similarity score</li>

 <li>Analyze the genome sequences</li>

 <li>Quit</li>

</ol>

4 Good bye!







Below is an example of running the main program.

<table width="624">

 <tbody>

  <tr>

   <td width="624">Select a numerical option:=== menu ===1.  Find similarity score2.  Find the best similarity score3.  Analyze the genome sequences4.  Quit<strong>1 </strong>Enter sequence 1: <strong>ATTCT </strong>Enter sequence 2:<strong>TAACT </strong>Similarity score: 0.4Select a numerical option:=== menu ===1.  Find similarity score2.  Find the best similarity score3.  Analyze the genome sequences4.  Quit<strong>2 </strong>Enter genome:<strong>ATTCCCTAA </strong>Enter sequence:<strong>TAC </strong>Best similarity score: 0.666667Select a numerical option:=== menu ===1.  Find similarity score2.  Find the best similarity score3.  Analyze the genome sequences4.  Quit<strong>3 </strong>Enter genome 1: <strong>ACCTT </strong>Enter genome 2: <strong>TCCTT </strong>Enter genome 3: <strong>TCCTT </strong></td>

  </tr>

 </tbody>

</table>

Enter sequence:

<strong>CCT </strong>

Genome 1 is the best match.

Genome 2 is the best match.

Genome 3 is the best match.

Select a numerical option:

=== menu ===

<ol>

 <li>Find similarity score</li>

 <li>Find the best similarity score</li>

 <li>Analyze the genome sequences</li>

 <li>Quit</li>

</ol>

<strong>6 </strong>

Invalid option.

Select a numerical option:

=== menu ===

<ol>

 <li>Find similarity score</li>

 <li>Find the best similarity score</li>

 <li>Analyze the genome sequences</li>

 <li>Quit</li>

</ol>

<strong>4 </strong>

Good bye!




Once you have tested your code on Cloud 9 / VS code,  then head over to code runner on Moodle and paste the entire program (functions from questions 4 – 6 and the main​         function from​  this question 7) in to the answer box!


