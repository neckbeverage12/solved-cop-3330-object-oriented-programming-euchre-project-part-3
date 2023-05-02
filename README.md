Download Link: https://assignmentchef.com/product/solved-cop-3330-object-oriented-programming-euchre-project-part-3
<br>
<strong>Assignment Scope</strong>

<ol>

 <li>Update classes due to changing requirements</li>

 <li>Use class Random</li>

 <li>Use an Iterator</li>

 <li>Add methods to classes to accomplish specific tasks</li>

 <li>Compile and run a project</li>

 <li>Compress a project and submit to Webcourses</li>

 <li>Decompress compressed project and verify it is a Netbeans project</li>

</ol>




<strong>References</strong>

<ol>

 <li>docx</li>

 <li>Setting up a project in Netbeans.docx</li>

 <li>Netbeans right click menu help.docx</li>

</ol>

<strong> </strong>

<strong>Deliverables</strong>

To complete this assignment you must submit your <strong>compressed Netbeans project </strong>to Webcourses.

<strong> </strong>

<strong>Tasks</strong>

<table width="667">

 <tbody>

  <tr>

   <td colspan="2" width="667"><strong>Activity</strong></td>

  </tr>

  <tr>

   <td width="181"><strong>Euchre project</strong></td>

   <td width="486"> </td>

  </tr>

  <tr>

   <td width="181"><strong>Euchre class</strong></td>

   <td width="486"> </td>

  </tr>

  <tr>

   <td width="181"><strong>constants</strong></td>

   <td width="486"> </td>

  </tr>

  <tr>

   <td width="181"><strong>Constants class</strong></td>

   <td width="486">Add the following constants1.      int ONE = 02.      int TWO = 13.      int NUM_PLAYERS = 44.      int DEAL_ONE = 25.      int DEAL_TWO = 3</td>

  </tr>

  <tr>

   <td width="181"><strong>core package</strong></td>

   <td width="486"> </td>

  </tr>

  <tr>

   <td width="181"><strong>AiPlayer class</strong></td>

   <td width="486"> </td>

  </tr>

  <tr>

   <td width="181"><strong>Card class</strong></td>

   <td width="486"> </td>

  </tr>

  <tr>

   <td width="181"><strong>Deck class</strong></td>

   <td width="486">Update class to1.      If not already included, generate getter/setter for member variable of data type Set&lt;Card&gt; that represents the deck of cards for the game</td>

  </tr>

  <tr>

   <td width="181"><strong>Game class</strong></td>

   <td width="486">Update class to1.      Add member variablesa.       Modify member variable named trump to be of data type class Card instead of enumeration Suitb.      Add member variable of data type class ArrayList specifically to only allow for instances of class Player that represents the game table layout (i.e. players of the game Euchre are set up so that team members sit across from each other, therefore the deal would be similar to TeamOne.PlayerOne, TeamTwo.PlayerOne, TeamOne.PlayerTwo, TeamTwo.PlayerTwo depending upon who the dealer is)c.       Add member variable of data type int to represent an integer index of the current dealer based on the table layoutd.      Add member variable of data type int to represent an integer index of the lead player based on the table layout2.      Update custom constructor to call methods AFTER existing method callsa.       setTableb.      dealHandc.       displayHands3.      Write method setTable to do the following:a.       Return type voidb.      Empty parameter listc.       Instantiate the member variable that represents the player table that is of data type ArrayListd.      Instantiate two instances of class Team set equal to each instance of class Team stored in the member variable of data type class ArrayList specifically of data type class Teame.       Instantiate four instances of class Player set equal to each instance of class Player stored in the member variable in class Team of data type class ArrayList of data type class Player(i.e. players of the game Euchre are set up so that team members sit across from each other, therefore the deal would be similar to TeamOne.PlayerOne, TeamTwo.PlayerTwo, TeamOne.PlayerTwo, TeamTwo.PlayerTwo depending upon who the dealer is)i.      There should be an instance of class Player that represents TeamOne, PlayerOneii.      There should be an instance of class Player that represents TeamOne, PlayerTwoiii.      There should be an instance of class Player that represents TeamTwo, PlayerOneiv.      There should be an instance of class Player that represents TeamTwo, PlayerTwof.        Explicitly add each player to the member variable that represents the game table, from above in an alternating pattern so that a player from TeamOne is added, followed by a player from TeamTwo, followed by a player from TeamOne, followed by a player from TeamTwo; this requires using the method signature of class ArrayList.add that requires two arguments; the first argument is the position in the ArrayList (i.e. 0, 1, 2, 3), the second argument is the object of data type class Player (e.g. table.add(0, teamOnePlayerOne)4.      Write method setDealerAndLead to do the followinga.       Instantiate an instance of class Randomb.      Set the member variable of primitive data type int that will represent a random integer of four players to determine who the initial dealer of the game is set equal to the method call .nextInt passing as an argument the value of the number of players in the game (i.e. four)c.       Set the member variable that represents the current dealer equal to the randomly selected value from item f. above using the .get method in class ArrayList on the member variable that represents the Euchre table5.       Write method dealHand to do the followinga.       Return type voidb.      Empty parameter listc.       Call method setDealerAndLeadd.      Create a local variable of data type int to represent the current player index initialized to the leadIdx member variablee.       Create a local variable of data type class Iterator explicitly only allowing for members of class Card set equal to member variable deck, calling method getDeck followed by method getIteratorf.        For the first deal of two cards each, loop through the number of playersi.      Call method dealOne passing as arguments the variables player index and the iteratorii.      If the current player value is greater than 3, reset the variable to the value of 0; otherwise increment the current playerg.      For the second deal of three cards each, loop through the number of playersi.      Call method dealTwo passing as arguments the variables player index and the iteratorii.      If the current player value is greater than 3, reset the variable to the value of 0; otherwise increment the current playerh.      Set the member variable trump equal to the next card on the deck6.      Write method dealOne so it does the followinga.       Return type voidb.      Receives two parametersi.      Data type int representing the current player indexii.      Data type Iterator&lt;Card&gt; representing the iteratorc.       Loops twicei.      Checks if the iterator has a next Card1.      Instantiate an instance of class Card set equal to method call next on the parameter iterator2.      Outputs to the console the dealt card and the player it was dealt to3.      Adds the card to the player’s hand by calling method getHand followed by method add, on the player instance stored at the parameter index location of member variable tableii.      Remove the current card from the HashSet using method call remove7.      Write method dealTwo so it does the followinga.       Return type voidb.      Receives two parametersi.      Data type int representing the current player indexii.      Data type Iterator&lt;Card&gt; representing the iteratorc.       Loops thricei.      Checks if the iterator has a next Card1.      Instantiate an instance of class Card set equal to method call next on the parameter iterator2.      Outputs to the console the dealt card and the player it was dealt to3.      Adds the card to the player’s hand by calling method getHand followed by method add, on the player instance stored at the parameter index location of member variable tableii.      Remove the current card from the HashSet using method call remove8.      Write method displayHands to do the followinga.       Loops through the game teamsi.      Call method outputHands in class Team</td>

  </tr>

  <tr>

   <td width="181"><strong>HumanPlayer class</strong></td>

   <td width="486"> </td>

  </tr>

  <tr>

   <td width="181"><strong>IPlayer interface</strong></td>

   <td width="486"> </td>

  </tr>

  <tr>

   <td width="181"><strong>Player class</strong></td>

   <td width="486">Update class to1.      Add member variable of data type class ArrayList specifically only allowing for instances of class Card that represents the player’s hand2.      Generate getter/setter for the member variable above representing the player’s hand3.      Write a customer constructor thata.       Receives no parametersb.      Instantiates the member variable of type ArrayList representing the player’s hand4.      Write method displayHanda.       Return type voidb.      Empty parameter listc.       Using an enhanced for loop, loop through the hand of the playeri.      Output to the console the face and suit of each card in the player’s hand</td>

  </tr>

  <tr>

   <td width="181"><strong>Team class</strong></td>

   <td width="486">Update class to1.      If it isn’t already included, add member variable of data type class String to represent the team’s name2.      Generate getter/setter for member variable representing the team’s name3.      Write method outputHandsa.       Return type voidb.      Empty parameter listc.       Using an enhanced for loop, loop through the collection of class Teami.      Call method outputHands for each player</td>

  </tr>

  <tr>

   <td width="181"><strong>userinterface package</strong></td>

   <td width="486"> </td>

  </tr>

  <tr>

   <td width="181"><strong>Euchre application</strong></td>

   <td width="486"> </td>

  </tr>

  <tr>

   <td width="181"><strong>Test Case 1</strong></td>

   <td width="486">Test Case 1 passes</td>

  </tr>

  <tr>

   <td width="181"><strong>Test Case 2</strong></td>

   <td width="486">Test Case 2 passes</td>

  </tr>

  <tr>

   <td width="181"><strong>Test Case 3</strong></td>

   <td width="486">Test Case 3 passes</td>

  </tr>

  <tr>

   <td width="181"><strong>Test Case 4</strong></td>

   <td width="486">Test Case 4 passes</td>

  </tr>

  <tr>

   <td width="181"><strong>Test Case 5</strong></td>

   <td width="486">Test Case 5 passes</td>

  </tr>

  <tr>

   <td width="181"><strong>Test Case 6</strong></td>

   <td width="486">Test Case 6 passes</td>

  </tr>

  <tr>

   <td width="181"><strong>Test Case 7</strong></td>

   <td width="486">Test Case 7 passes</td>

  </tr>

  <tr>

   <td width="181"><strong> </strong></td>

   <td width="486">Source compiles with no errors</td>

  </tr>

  <tr>

   <td width="181"><strong> </strong></td>

   <td width="486">Source runs with no errors</td>

  </tr>

  <tr>

   <td width="181"><strong> </strong></td>

   <td width="486">Source includes comments</td>

  </tr>

 </tbody>

</table>

<strong> </strong>

<strong>Perform the following test cases</strong>

<table width="638">

 <tbody>

  <tr>

   <td colspan="3" width="638"><strong>Test Cases</strong></td>

  </tr>

  <tr>

   <td width="166"><strong> </strong></td>

   <td width="166"><strong>Action</strong></td>

   <td width="307"><strong>Expected outcome</strong></td>

  </tr>

  <tr>

   <td width="166"><strong>Test Case 1</strong></td>

   <td width="166"><strong>Project view</strong></td>

   <td width="307">Completed project view should look like figure 1</td>

  </tr>

  <tr>

   <td width="166"><strong>Test case 2</strong></td>

   <td width="166"><strong>Regression testing; Run application</strong></td>

   <td width="307">The console window should look like figure 2</td>

  </tr>

  <tr>

   <td width="166"><strong>Test case 3</strong></td>

   <td width="166"><strong>Regression testing; Run application </strong></td>

   <td width="307">The JOptionPane.showMessageDialog() method call should look like figure 3</td>

  </tr>

  <tr>

   <td width="166"><strong>Test case 4</strong></td>

   <td width="166"><strong>Regression testing; Run application</strong></td>

   <td width="307">The console window should look similar to figure 4 for the initial display of the deck of cards</td>

  </tr>

  <tr>

   <td width="166"><strong>Test case 5</strong></td>

   <td width="166"><strong>Regression testing; Run application</strong></td>

   <td width="307">The output in the console window should display the deck of cards after being shuffled and should NOT be in the same order as the first output, similar to figure 5</td>

  </tr>

  <tr>

   <td width="166"><strong>Test case 6</strong></td>

   <td width="166"><strong>Run application</strong></td>

   <td width="307">The output in the console window should display the hands of team one after the deal, similar to figure 6</td>

  </tr>

  <tr>

   <td width="166"><strong>Test case 7</strong></td>

   <td width="166"><strong>Run application</strong></td>

   <td width="307">The output in the console window should display the hands of team one after the deal, similar to figure 7</td>

  </tr>

  <tr>

   <td width="166"><strong>Test case 8</strong></td>

   <td width="166"><strong>Run application</strong></td>

   <td width="307">The output in the console window should display the hands of team one after the deal, similar to figure 8</td>

  </tr>

  <tr>

   <td width="166"><strong>Test case 9</strong></td>

   <td width="166"><strong>Run application </strong></td>

   <td width="307">The output in the console window should display the hands of team two after the deal, similar to figure 9</td>

  </tr>

  <tr>

   <td width="166"><strong>Test case 10</strong></td>

   <td width="166"><strong>Run application</strong></td>

   <td width="307">The output in the console window should display the hands of team two after the deal, similar to figure 10</td>

  </tr>

 </tbody>

</table>

<strong> </strong>

<strong> </strong>

Figure 1 Project View




Figure 2 Output in console window




Figure 3 Display from JOptionPane.showMessageDialog() method




Figure 4 Initial display of deck of cards




Figure 5 Display of deck of cards after shuffle




Figure 6 Display of First Deal

Figure 7 Display of Second Deal




Figure 8 Display of Trump




Figure 9 Team One Player’s Hands




Figure 10 Team Two Player’s Hands







Figure 11 Table Layout for Euchre