# Campo_J_Garcia_C_Golfscript

GolfScript is a language made for a particular reason, yet the purpose is more on entertainment than its effectiveness. It is mostly used in Code Golf competitions where you want to use a program that's as small as possible. It does not have several built-in functions, and is stack-based. Programmers don't need to use variables or function names explicitly. Using stack minimizes the amount of syntax overhead. Values and functions are pushed on the stack, then operators pop values from the stack and manipulate them.

Types (order in smallest to largest priority):
1. Integers
2. Arrays
3. Strings
4. Blocks

Some of the built-ins in Golfscript:


|Built-ins |Application |Example|Output|
|----------|------------|-------|------|
|+ |Addition / concat|1 2 +|3|
|* | multiplication |1 2 * |2 |
| |Array/string repeat |[1 2 ] 2 * | [1 2 1 2] |
| |join | [1 2 3] ‘,’ * | “1,2,3”|
| |fold | [1 2 3 4]{+}* | 10 |
|! | not |1! |0 |
|% |Modulus |7 3 %| 1|
| | Map | [1 2 3]{1+}% | [2 3 4] |
|; |pop/discard |1 2 3; |1 2 |
|,| Array of n elements | 5, | [0 1 2 3 4] |
|. |Duplicate top of stack |1 2. |1 2 2 |
|(|decrement |2( | 1 |
|)|increment | 2) | 3 |

Example:
Input: 2 3 +

Output: 5

It would push 2 onto the stack, then 3, then pop them both, add them together, and push 5 on the stack. 

Input: {.!{1}{,{)}%{*}*}if}:fact;
       5fact

Output: 120


References:

Golfscript Tutorial. (n.d.).  Golfscript. Retrieved from: http://www.golfscript.com/golfscript/index.html

Roche, D. (2021, November 17).  Golfscript. USNA. https://www.usna.edu/Users/cs/roche/413/proj/golfscript.php

Wayne, H. (2021, May 16).  A BRIEF INTRODUCTION TO ESOTERIC LANGUAGES. Hillel Wayne. https://www.hillelwayne.com/talks/esolangs/











