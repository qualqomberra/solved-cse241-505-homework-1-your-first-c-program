Download Link: https://assignmentchef.com/product/solved-cse241-505-homework-1-your-first-c-program
<br>
You will write a C++ program that will play the game of HEX. The game of Hex is played by two players (computer-user or user1-user2) on a two-dimensional board (2D C array) with hexagonal cells (each cell has 6 neighbors: east, west, northeast, northwest, southeast, southwest). The neighbors of F3 are G2, F2, E3, E4, F4, and G3. Each cell is either occupied by computer (user1), user (user2) or empty. The game starts with the following board for an 8×8 game:




a b c d e f g h

<ul>

 <li>. . . . . . . .</li>

 <li>. . . . . . . .</li>

 <li>. . . . . . . .</li>

 <li>. . . . . . . .</li>

 <li>. . . . . . . .</li>

 <li>. . . . . . . .</li>

 <li>. . . . . . . .</li>

 <li>. . . . . . . .</li>

</ul>




where ‘<strong>.’</strong> represents the empty cells, ‘<strong>x’</strong> represents the computer(user1) cells and ‘<strong>o’</strong> represents the user (user2) cells. Please see <a href="https://www.maths.ed.ac.uk/~csangwin/hex/index.html">https://www.maths.ed.ac.uk/~csangwin/hex/index.html</a> for the rules of the game (we will ignore the swap rule). The following is a board from <a href="http://www.iggamecenter.com/">http://www.iggamecenter.com/</a><a href="http://www.iggamecenter.com/">.</a> There is playable game available at <a href="http://www.lutanho.net/play/hex.html">http://www.lutanho.net/play/hex.html</a>



















The players take turns to play the game. For the above board, the user can pick any cell to put the first piece.  For example, if the user1 plays to cell C5 and user2 plays to letter F3 then the board becomes

a b c d e f g h 1 . . . . . . . .

<ul>

 <li>. . . . . . . .</li>

 <li>. . . . . o . .</li>

 <li>. . . . . . . .</li>

 <li>. . x . . . . .</li>

 <li>. . . . . . . .</li>

 <li>. . . . . . . . 8        . . . . . . . .</li>

</ul>







The game continues with the objective of “The first player to form a connected path of their marks linking the opposing sides of the board marked by their color wins.” For example, in the following board, the user1 wins because he/she connects the blue (numbers) sides. The winning path is marked with capital X and O.

a b c d e f g h 1 . . . . o . . .

<ul>

 <li>. . . . o o . .</li>

 <li>. . . . . o . .</li>

 <li>. . o X X o X X 5     . . X o X X . .</li>

 <li>X X o . . . . .</li>

 <li>. o . . . x . . 8        . o . . x . . .</li>

</ul>
















Your program will do the followings:

<ol>

 <li>When your program starts, you will ask the user for the board size. The board size can be 6×6, 7×7, 8×8, 9×9, 10×10, 11×11 or 12×12. You should check whether the input size is valid or not.</li>

 <li>Ask the user if this a two player game or user versus computer game.</li>

 <li>You will display the initial board. We will ignore the swap rule of the game.</li>

 <li>You ask the user to make a move, get the user move from the keyboard and draw the new board. Use positions such as A 1, B 7, C 10, etc. If the move is not legal, then ask for another move.</li>

 <li>The computer (or user2) makes a new move and draws the board again. You should print what move the computer chose on the screen. The move should be legal and try to make it “smart”. In other words, chose the legal move that wins the largest number of cells instead of other moves. For the smart moves, use the suggested strategies described at <a href="https://www.maths.ed.ac.uk/~csangwin/hex/index.html">https://www.maths.ed.ac.uk/~csangwin/hex/index.html</a></li>

 <li>The game continues until all the board is filled or one of the players wins.</li>

 <li>The final result of the game should be printed on the screen showing who won and the connected cells with upper case O and X.</li>

</ol>







Notes:

<ul>

 <li>Do not use any functions from the standard C library (like <strong><sub>printf</sub></strong>)</li>

 <li>Your program should have only functions and no classes.</li>

 <li>Do not forget to indent your code and provide comments.</li>

 <li>Check the validity of the user input.</li>

 <li><strong><u>Test your programs very carefully at least with 10 different runs. For some runs, let the</u> <u>computer win and for others the user should win. There should be cases for illegal moves</u> <u>and your program should handle them appropriately.</u> </strong></li>

 <li>You should submit your work to the Moodle page. We will post the submission rules soon which should be strictly followed.</li>

</ul>