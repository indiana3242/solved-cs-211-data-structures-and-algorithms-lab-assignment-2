Download Link: https://assignmentchef.com/product/solved-cs-211-data-structures-and-algorithms-lab-assignment-2
<br>
The objective of this assignment is to implement Binary Search Tree (BST).

<strong> </strong>

<strong>Command-line argument:</strong>

Your program should receive a file (input file) as a command line argument.




<h1>Input file</h1>

The input file will be a text file where each line will be of any of the following format:

insert &lt;number&gt;, inorder, preorder, postorder, search &lt;number&gt;, minimum, maximum, successor &lt;number&gt;, predecessor &lt;number&gt;, delete &lt;number&gt;, where &lt;number&gt; represents any non-negative integer. The input will be given in such a way that, at any point in time, the BST contains only distinct numbers.




The output must be in a file named ‘bst.txt’. Every line in the input file must have a corresponding output line in bst.txt. The details are given below.




<table width="564">

 <tbody>

  <tr>

   <td width="167"><strong>Command </strong></td>

   <td width="145"><strong>Meaning </strong></td>

   <td width="252"><strong>Output </strong></td>

  </tr>

  <tr>

   <td width="167">insert &lt;number&gt;</td>

   <td width="145">Insert &lt;number&gt; to the BST</td>

   <td width="252">&lt;number&gt; inserted</td>

  </tr>

  <tr>

   <td width="167">inorder</td>

   <td width="145">Do an inorder traversal of the BST</td>

   <td width="252">Sequence of numbers (separated by a white space) obtained by doing inorder traversal / &lt;empty-line&gt; (ifBST is empty)</td>

  </tr>

  <tr>

   <td width="167">preorder</td>

   <td width="145">Do a preorder traversal of the BST</td>

   <td width="252">Sequence of numbers (separated by a white space) obtained by doing preorder traversal / &lt;empty-line&gt; (ifBST is empty)</td>

  </tr>

  <tr>

   <td width="167">postorder</td>

   <td width="145">Do a post-order traversal of the BST</td>

   <td width="252">Sequence of numbers (separated by a white space) obtained by doing postorder traversal / &lt;empty-line&gt; (ifBST is empty)</td>

  </tr>

  <tr>

   <td width="167">search &lt;number&gt;</td>

   <td width="145">Search &lt;number&gt; in the BST</td>

   <td width="252">&lt;number&gt; found / &lt;number&gt; not found</td>

  </tr>

  <tr>

   <td width="167">minimum</td>

   <td width="145">Obtain the minimum number in the BST</td>

   <td width="252">&lt;minimum-number&gt; / &lt;empty-line&gt;(if BST is empty)</td>

  </tr>

  <tr>

   <td width="167">maximum</td>

   <td width="145">Obtain the</td>

   <td width="252">&lt;maximum-number&gt; / &lt;empty-line&gt;</td>

  </tr>

  <tr>

   <td width="167"> </td>

   <td width="145">maximum number in the BST</td>

   <td width="252">(if BST is empty)</td>

  </tr>

  <tr>

   <td width="167">successor &lt;number&gt;</td>

   <td width="145">Obtain the successor of &lt;number&gt; in theBST</td>

   <td width="252">&lt;successor&gt; / &lt;number&gt; does not exist / successor of &lt;number&gt; doesnot exist (if &lt;number&gt; is the maximum number)</td>

  </tr>

  <tr>

   <td width="167">predecessor &lt;number&gt;</td>

   <td width="145">Obtain the predecessor of &lt;number&gt; in theBST</td>

   <td width="252">&lt;predecessor&gt; / &lt;number&gt; does not exist / predecessor of &lt;number&gt;does not exist (if &lt;number&gt; is theminimum number) </td>

  </tr>

  <tr>

   <td width="167">delete &lt;number&gt;</td>

   <td width="145">Delete (if exists)&lt;number&gt; from theBST</td>

   <td width="252">&lt;number&gt; deleted / &lt;number&gt; does not exist</td>

  </tr>

 </tbody>

</table>




The content of an example input file (on the left side) and the corresponding output file (on the right side) are given below.




<table width="592">

 <tbody>

  <tr>

   <td width="321">insert 6</td>

   <td colspan="3" width="271">6 inserted</td>

  </tr>

  <tr>

   <td width="321">insert 9</td>

   <td colspan="3" width="271">9 inserted</td>

  </tr>

  <tr>

   <td width="321">insert 3</td>

   <td colspan="3" width="271">3 inserted</td>

  </tr>

  <tr>

   <td width="321">insert 19</td>

   <td colspan="3" width="271">19 inserted</td>

  </tr>

  <tr>

   <td width="321">insert 0</td>

   <td colspan="3" width="271">0 inserted</td>

  </tr>

  <tr>

   <td width="321">insert 5</td>

   <td colspan="3" width="271">5 inserted</td>

  </tr>

  <tr>

   <td width="321">inorder</td>

   <td colspan="3" width="271">0 3 5 6 9 19</td>

  </tr>

  <tr>

   <td width="321">preorder</td>

   <td colspan="3" width="271">6 3 0 5 9 19</td>

  </tr>

  <tr>

   <td width="321">search 6</td>

   <td colspan="3" width="271">6 found</td>

  </tr>

  <tr>

   <td width="321">search 8</td>

   <td colspan="3" width="271">8 not found</td>

  </tr>

  <tr>

   <td width="321">delete 10</td>

   <td colspan="3" width="271">10 does not exist</td>

  </tr>

  <tr>

   <td width="321">delete 9</td>

   <td colspan="3" width="271">9 deleted</td>

  </tr>

  <tr>

   <td width="321">insert 21</td>

   <td colspan="3" width="271">21 inserted</td>

  </tr>

  <tr>

   <td width="321">insert 13</td>

   <td colspan="3" width="271">13 inserted</td>

  </tr>

  <tr>

   <td width="321">maximum</td>

   <td colspan="3" width="271">21</td>

  </tr>

  <tr>

   <td width="321">minimum</td>

   <td colspan="3" width="271">0</td>

  </tr>

  <tr>

   <td width="321">postorder</td>

   <td colspan="3" width="271">0 5 3 13 21 19 6</td>

  </tr>

  <tr>

   <td width="321">successor 4</td>

   <td colspan="3" width="271">4 does not exist</td>

  </tr>

  <tr>

   <td width="321">predecessor 19</td>

   <td colspan="3" width="271">13</td>

  </tr>

  <tr>

   <td width="321">predecessor 0</td>

   <td colspan="3" width="271">predecessor of 0 does not exist</td>

  </tr>

  <tr>

   <td width="321">delete 0</td>

   <td colspan="3" width="271">0 deleted</td>

  </tr>

  <tr>

   <td width="321">delete 3</td>

   <td colspan="3" width="271">3 deleted</td>

  </tr>

  <tr>

   <td width="321">delete 5</td>

   <td colspan="3" width="271">5 deleted</td>

  </tr>

  <tr>

   <td width="321">delete 6</td>

   <td colspan="3" width="271">6 deleted</td>

  </tr>

  <tr>

   <td width="321">delete 19</td>

   <td colspan="3" width="271">19 deleted</td>

  </tr>

  <tr>

   <td width="321">delete 13</td>

   <td colspan="3" width="271">13 deleted</td>

  </tr>

  <tr>

   <td colspan="2" width="384">delete 21</td>

   <td width="111">21 deleted</td>

   <td width="97"> </td>

  </tr>

  <tr>

   <td colspan="2" width="384">delete 1</td>

   <td width="111">1 does not exist</td>

   <td width="97"> </td>

  </tr>

  <tr>

   <td colspan="2" width="384">inorder</td>

   <td width="111"> </td>

   <td width="97"> </td>

  </tr>

  <tr>

   <td colspan="2" width="384">insert 1</td>

   <td width="111">1 inserted</td>

   <td width="97"> </td>

  </tr>

  <tr>

   <td colspan="2" width="384">inorder</td>

   <td width="111">1</td>

   <td width="97"> </td>

  </tr>

  <tr>

   <td width="321"></td>

   <td width="64"></td>

   <td width="111"></td>

   <td width="97"></td>

  </tr>

 </tbody>

</table>

<strong> </strong>

You can follow your own pseudocode for implementing these functions. But the ‘effect’ should be the same as that discussed in the class. For example, we know that a node can potentially be inserted at many places in a BST. But for this assignment, it is required that the node should be inserted at the leaf, as discussed in the class.




<h1>Submission</h1>

<ul>

 <li>The program you submit should output bst.txt when run.</li>

 <li>The main file of your program should be named as &lt;roll no&gt;.&lt;extension&gt;, where roll no. specifies your roll no. and the extension depends on the language you choose (Usage of C/C++ is mandatory for this assignment). Ex: 180040001.c</li>

 <li>Test well before submission. We have some hidden inputs with us to test your program. The mark you obtain is purely based on whether your program correctly gives outputs for the hidden inputs.</li>

 <li>If your program has only a single source file, please submit the file as it is. If your program has multiple source files, please submit your code as a zip file where the name of the zip file should be your roll number. It is important that you follow the input/output conventions exactly (including the naming scheme) as we may be doing an automated evaluation. There will be a penalty of 10% (on the mark you deserve otherwise) if you do not follow the naming conventions exactly.</li>

 <li>Follow some coding style uniformly. Provide proper comments in your code.</li>

 <li>Submit only through moodle. Submit well in advance. Any hiccups in the moodle/internet at the last minute is never acceptable as an excuse for late submission. Submissions through email or any other means will be ignored.</li>

 <li>Acknowledge the people (other than the instructor and TA) who helped you to solve this assignment. The details of the help you received and the names of the people who helped you (including internet sources, if applicable) should come in the beginning of the main file as a comment. Copying others’ programs is a serious offence and deserving penalty will be imposed if found.</li>

</ul>


