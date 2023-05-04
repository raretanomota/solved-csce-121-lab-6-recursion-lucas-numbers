Download Link: https://assignmentchef.com/product/solved-csce-121-lab-6-recursion-lucas-numbers
<br>
This lab will give you some practice with recursion (in the first question) and also processing file input (in the second one).

How far must I get?

There are fewer questions this week to make it easier for everyone to finish. Please try your best to do so!

Recursion: Lucas numbers

No doubt you’ll have heard of the Fibonacci series. <a href="https://en.wikipedia.org/wiki/%C3%89douard_Lucas">François Lucas</a> was the person who made them famous and a closely related series of numbers were named for him. With the elements denoted <em>L<sub>i</sub></em>, his series begins thus: <em>L<sub>0</sub>=2</em>, <em>L<sub>1</sub>=1</em>, <em>L<sub>2</sub>=3</em>, <em>L<sub>3</sub>=4</em>, <em>L<sub>4</sub>=7</em>, …The definition for a general element in the series is recursive, as follows:

<ol>

 <li>Write a recursive function that computes the <em>n<sup>th</sup></em> element, <em>L<sub>n</sub></em>.</li>

 <li>Now call your previous function to compute the value of <em>L<sub>n</sub></em>/<em>L<sub>n-</sub></em><em><sub>1</sub></em>. Increase the value of <em>n</em> until this ratio changes by a factor less than <em>10<sup>-4</sup></em>.</li>

</ol>

iii. If you try to compute <em>L<sub>50</sub></em> with your function, you’ll probably find that it takes an unreasonably long time to return a result. An important question is: for a particular <em>n</em>, how many times is the function called? Modify your code from the first part, instrumenting it so that it also counts the number of function calls. Can you figure out how to express this count (i.e., the total number of function calls) in terms of <em>n</em>?

<ol>

 <li>Rather than merely calling your recursive function, what is a more efficient way to compute large Lucas numbers?</li>

</ol>

<h2>Sentences of moderate length please!</h2>

Some students have said they find my questions too wordy. This question involves writing some code that will help me examine my writing style, by selecting only those sentences that are of moderate length.

Write a program that prints out all the sentences in a text file where: min ≤ <em>length</em> ≤ max.Assume that a sentence ends in either a period, question mark, or exclamation point. Count all the blanks and punctuation in computing <em>length</em>, with the exception of any spaces separating one sentence from the next. (All end-of-line characters, i.e. the ‘
’, should simply be ignored.)

You can also assume that every line in the file has fewer than 200 characters. However, you can’t assume any bound on the length of the sentences in the file—so you shouldn’t try store it all in a single char array. Nor should you assume any maximum on the total number of sentences.

Request the filename and also min and max values as inputs from the user. Ensure that they are positive integers with min ≤ max &lt; 1000.

<table>

 <tbody>

  <tr>

   <td>

    <table>

     <tbody>

      <tr>

       <td><strong>?</strong></td>

       <td>HINT</td>

      </tr>

     </tbody>

    </table></td>

   <td>

    <table>

     <tbody>

      <tr>

       <td>Start by writing some code that will print the file sentence by sentence whilst respecting the constraint that you can’t store the whole thing in a single char[].</td>

      </tr>

     </tbody>

    </table></td>

  </tr>

  <tr>

   <td>

    <table>

     <tbody>

      <tr>

       <td><strong>?</strong></td>

       <td>HINT</td>

      </tr>

     </tbody>

    </table></td>

   <td>

    <table>

     <tbody>

      <tr>

       <td>Write a function that processes just one character. Also, this problem is a case where using global variables might be a good idea.</td>

      </tr>

     </tbody>

    </table></td>

  </tr>

 </tbody>

</table>




<table>

 <tbody>

  <tr>

   <td>

    <table>

     <tbody>

      <tr>

       <td><strong>?</strong></td>

       <td>TESTING IDEAS</td>

      </tr>

     </tbody>

    </table></td>

   <td>

    <table>

     <tbody>

      <tr>

       <td>Remember to test your code on an empty file, and also one with just a single punctuation mark. Finally, consider a file in which the final sentence in the file is missing its ending punctuation.</td>

      </tr>

     </tbody>

    </table></td>

  </tr>

 </tbody>

</table>

<h2>Puzzling*</h2>

Here’s a question to think about:

Is it possible to fill an 8×8 grid with dominoes (2×1 in size) such that no two dominoes form a 2×2 square?