Download Link: https://assignmentchef.com/product/solved-comp2140-lab4-simulating-a-simple-survivor-game-with-a-queue
<br>
To simulate a simple survivor game with a queue.

<strong>Exercise</strong>

File Lab4.java contains an almost-complete application with a simple Queue. You need to add most of the body of the method survivor, which currently only prints some information.

The survivor method should simulate (using a queue) the survivor game. In this game, <em>N </em>people (numbered 0 to <em>N</em>− 1) stand in circle, then every <em>k</em>th person is counted out (leaves the circle), until only one person is left. At each elimination, you should print out the eliminated person’s number.

For example, if there are 7 people (<em>N </em>= 7) and <em>k </em>= 2, then you should print out 1 3 5 0 4 2 6 because

<table width="484">

 <tbody>

  <tr>

   <td width="294">the circle changes as follows:</td>

   <td width="70"> </td>

   <td width="120"> </td>

  </tr>

  <tr>

   <td width="294">0</td>

   <td width="70">0</td>

   <td width="120">0</td>

  </tr>

 </tbody>

</table>

6                                  1                 6                 1                 6

<ul>

 <li>2 5              2              5               2</li>

</ul>

4                       3                             4                       3                             4                       3

Start                                  First elimination: 1                  Second elimination: 3

0                                                      0

<ul>

 <li>6 6</li>

</ul>

<table width="457">

 <tbody>

  <tr>

   <td width="140">4Third elimination: 5</td>

   <td width="163">4Fourth elimination: 0</td>

   <td width="32"> </td>

   <td width="122">4Fifth elimination: 4</td>

  </tr>

  <tr>

   <td width="140">6</td>

   <td width="163"> </td>

   <td width="32">6</td>

   <td width="122"> </td>

  </tr>

 </tbody>

</table>

5                  2                                                      2                          2

2

Third elimination: 2             Last element remaining: 6

The code that you add to the survivor method must simulate the game using a queue to represent the circle of people. To do the eliminating, you must use the standard queue methods (enter, leave, front, and isEmpty) provided in the Queue class. You may not change the Queue class or the main method in any way.

Hint: You can keep eliminating until <em>no </em>people are left in the circle. Sample output:

7 people numbered 0 to 6 stand in a circle.

Every second person is eliminated repeatedly until only one person is left.

The people are eliminated in the following order:

1 3 5 0 4 2 6 &lt;=== last person left

11 people numbered 0 to 10 stand in a circle.

Every third person is eliminated repeatedly until only one person is left. The people are eliminated in the following order:

2 5 8 0 4 9 3 10 7 1 6 &lt;=== last person left

17 people numbered 0 to 16 stand in a circle.

Every 5-th person is eliminated repeatedly until only one person is left.

The people are eliminated in the following order:

4 9 14 2 8 15 5 12 3 13 7 1 0 6 11 16 10 &lt;=== last person left

Program ends normally.