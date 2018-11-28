**Unit 4: Game Playing** <span id="4"></span> 
*Some of the earliest and most recognizable AI applications are games
like chess and tic-tac-toe, the most famous being the chess match
between Garry Kasparov and Deep Blue.  In this unit, we will discuss the
development of game-playing applications, as well as the relationship
between game-playing and searching algorithms.  The unit will also
provide you with some best practices for building game programs.   
  
 Unit Note: This unit has been designed to teach you how to design
algorithms for game-playing applications.  For our purposes, you will
find tic-tac-toe, which uses features of search and constraint
satisfaction, the simplest.  We suggest that as an informal exercise,
you create a tic-tac-toe application and then play against it, noting
the algorithm's success rates and determining which modifications will
need to be implemented in order to improve its performance.*

**Unit 4 Time Advisory**  
This unit should take approximately 10 hours to complete.  
  
 ☐    Subunit 4.1: 1 hour  
  
 ☐    Subunit 4.2: 6 hours
  
 ☐    Subunit 4.2.1: 3 hours  
  
 ☐    <span class="Apple-style-span"
style="text-align: -webkit-auto; ">Subunit 4.2.2: 3 hours</span>

☐    Subunit 4.3: 3 hours

**Unit4 Learning Outcomes**  
Upon successful completion of this unit, the student will be able to:  
  
-   Delineate game playing in the history of AI.
-   Design algorithms for playing simple games.

**4.1 Background: Game Playing in AI** <span id="4.1"></span> 
-   **Reading: Wikipedia: “History of Artificial Intelligence”**
    Link: Wikipedia: ["History of Artificial
    Intelligence"](https://resources.saylor.org/wwwresources/archived/site/wp-content/uploads/2011/11/CS405-4.1-WIKIPEDIA.pdf)
    (PDF)  
        
     Instructions: Select the link and read optionally the history of
    artificial intelligence, but definitely read the sections on the
    Turing Test, games, checkers and chess.   
        
     These readings apply to sections 4.1.1–4.1.3 below.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-Share-Alike License
    3.0](http://creativecommons.org/licenses/by-sa/3.0/) (HTML).  You
    can find the original Wikipedia version of this article
    [here](http://en.wikipedia.org/wiki/History_of_artificial_intelligence)
    (HTML).

**4.1.1 Game Playing History** <span id="4.1.1"></span> 
-   **Reading: UCI: Max Welling’s ICS 17 Introduction to Artificial
    Intelligence Course: “Slides Lecture 1 (Intro)”**
    Link: UCI: Max Welling’s ICS 17 Introduction to Artificial
    Intelligence Course: “[Slides Lecture 1
    (Intro)](http://www.ics.uci.edu/~welling/teaching/ICS171spring07/ICS171spring07.html)”
    (PPT)  
        
     Instructions: Select the PowerPoint file slides lecture 1(Intro)
    and review slides 10, 11, and 15.  Game playing provided numerous
    applications that motivated the development of AI techniques—for
    example, search and problem-solving techniques.  In addition, it
    served as a popular benchmark for demonstrating progress and
    improvements of AI research.  
        
     Terms of Use: Please respect the copyright and terms of use
    displayed on the webpages above.

**4.1.2 Alan Turing and Checkers** <span id="4.1.2"></span> 
*Note: The readings of 4.1 and 4.1.1 apply to this subunit.  Arthur
Samuel's checkers-playing program is a famous example.*

**4.1.3 Garry Kasparov vs. IBM’s Deep Blue** <span id="4.1.3"></span> 
*Note: The readings of 4.1 and 4.1.1 apply to this subunit.  Kasparov
vs. IBM's Deep Blue is a famous chess match that demonstrated
master-level chess play by a machine.*

**4.2 Applicability of Search** <span id="4.2"></span> 
-   **Reading: Mark Watson’s Practical Artificial Intelligence
    Programming with Java: “Chapter 2: Search”**
    Link: Mark Watson’s *Practical Artificial Intelligence Programming
    with Java*: ["Chapter 2:
    Search"](https://resources.saylor.org/wwwresources/archived/site/wp-content/uploads/2011/11/CS405-1.1-WATSON.pdf) (PDF)  
        
     Instructions: Select the link above and read section 2.5 for ideas
    on programming searching, and implementing the ideas in Java
    programs for game playing.  Min-max is a search strategy for
    two-person games whereby a move is selected by choosing the child
    node that has either the maximum (a player strives to maximize
    his/her advantage) or minimum (a player strives to minimize the
    other player’s advantage).  Alpha-Beta search is an improvement of
    min-max searching by eliminating, or pruning, branches from the
    search tree.   
        
     This reading applies to sections 4.2.1 and 4.2.2.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-NoDerivs Unported License
    3.0](http://creativecommons.org/licenses/by-nc-nd/3.0/) (HTML).  It
    is attributed to Mark Watson and the original version can be found
    [here](http://markwatson.com/opencontent/JavaAI3rd.pdf) (PDF).

**4.2.1 Relation to Search** <span id="4.2.1"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 3: Constraint Satisfactory Problems
    (CSP) and Games2”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: ["Chapter 3: Constraint Satisfactory Problems (CSP) and
    Games2"](https://resources.saylor.org/wwwresources/archived/site/wp-content/uploads/2011/11/CS405-4.2.1-MIT.pdf)
    (PDF)   
        
     Instructions: Study slides 3.4.1–3.4.33 in 6.034 Notes: Section
    3.4, for the application of ideas presented so far on two-person
    games, like tic-tac-toe, checkers, and chess.   
        
     This reading applies to subsections 4.2.1.1–4.2.1.4, which define a
    tree structure for representing board games.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF).

**4.2.1.1 States: Board Positions** <span id="4.2.1.1"></span> 
*Note: The readings of 4.2.1 apply to this subunit.  The states of a
board game are the board positions or configurations of the game
pieces—for example, the chess pieces on the chessboard.  The states are
represented by the nodes of a tree.*

**4.2.1.2 Operators: Game Moves** <span id="4.2.1.2"></span> 
*Note: The readings of 4.2.1 apply to this subunit.  The game moves, or
operators, are represented by the arcs of a tree.*

**4.2.1.3 Goal State: Winning Position** <span id="4.2.1.3"></span> 
*Note: The readings of 4.2.1 apply to this subunit.  The goal state is a
goal node, i.e., the board configuration that depicts the winning
position of the game pieces.*

**4.2.1.4 Heuristics: Scoring Function** <span id="4.2.1.4"></span> 
*Note: The readings of 4.2.1 apply to this subunit.  In many games, the
size of the search tree can be very large and the complexity of the
search can be high.  Heuristics are used to guide the search, increase
efficiency, and improve game-playing ability*

**4.2.2 Min-Max Search and Alpha-Beta Search** <span id="4.2.2"></span> 
-   **Reading: UCI: Max Welling’s ICS 171 Introduction to Artificial
    Intelligence Course: “Slides Lecture 6 (Games)”**
    Link: UCI: Max Welling’s ICS 171 Introduction to Artificial
    Intelligence Course: “[Slides Lecture 6
    (Games)](http://www.ics.uci.edu/~welling/teaching/ICS171spring07/ICS171spring07.html)”
    (PPT)  
        
     Instructions: Select the PowerPoint file slides lecture 6 (Games)
    and read the slides.  MinMax and Alpha-Beta are fundamental search
    algorithms used in game playing.  
        
     Terms of Use: Please respect the copyright and terms of use
    displayed on the webpages above.

**4.3 Notes on Building Game Programs** <span id="4.3"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: "Chapter 3: Constraint Satisfactory Problems
    (CSP) and Games2"**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: ["Chapter 3: Constraint Satisfactory Problems (CSP) and
    Games2"](https://resources.saylor.org/wwwresources/archived/site/wp-content/uploads/2011/11/CS405-4.2.1-MIT.pdf)
    (PDF)  
        
     Instructions: Study slides 3.4.31–3.4.33 in 6.034 Notes: Section
    3.4, for practical considerations and observations.   
        
     This reading applies to subsections 4.3.1 and 4.3.2.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF).

**4.3.1 Computer Works Best When Game Rules are Clear** <span
id="4.3.1"></span> 
*Note: This subunit is addressed in the readings of 4.3.  The title of
this subunit gives one reason why game playing is a desirable
application domain for introductory AI investigation; namely, the
solution or goal has a precise specification. *

**4.3.2 Success Follows Long Periods of Gradual Refinement** <span
id="4.3.2"></span> 
*Note: This subunit is addressed in the readings of 4.3.  The title of
this subunit gives an indication of the difficulty of designing and
building a program that competes in difficult games at a high level. 
Either a revolutionary new algorithm is discovered, or improvements come
from small incremental steps learned from experimentation over a long
period of time.*


