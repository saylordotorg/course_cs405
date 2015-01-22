**Unit 2: Search** <span id="2"></span> 
*Previous coursework has familiarized you with searching algorithms.  In
this unit, you will learn how to implement standard searching
algorithms.  We will first discuss the motivation behind exploring
search from an AI perspective, learning new terminology as we go that
will be used in this unit and beyond.  We will then learn about basic
search methods, as well as time and memory requirements, concluding with
a discussion of the advantages and disadvantages of searching
algorithms.  By the end of this unit, you will be able to apply AI
techniques when developing searching algorithms.*

**Unit 2 Time Advisory**  
This unit should take approximately 12 hours to complete.  
  
 ☐    Subunit 2.1: 2 hours  
  
 ☐    Subunit 2.2: 8 hours
  
 ☐    Subunit 2.2.1: 2 hours  
  
 ☐    <span class="Apple-style-span"
style="text-align: -webkit-auto; ">Subunit 2.2.2: 2 hours</span>  
  
 ☐    <span class="Apple-style-span"
style="text-align: -webkit-auto; ">Subunit 2.2.3: 2 hours</span>  
  
 ☐    <span class="Apple-style-span"
style="text-align: -webkit-auto; ">S</span><span
class="Apple-style-span" style="text-align: -webkit-auto; ">ubunit
2.2.4: 2 hours</span>

☐    Subunit 2.3: 2 hours

**Unit2 Learning Outcomes**  
Upon successful completion of this unit, the student will be able to:  
  
-   Describe the role of search in AI.
-   Give examples of the basic types of search algorithms.
-   Explain the basic types of search algorithms.
-   Discuss the computational complexity of search algorithms.

**2.1 Motivation** <span id="2.1"></span> 
-   **Reading: Mark Watson’s Practical Artificial Intelligence
    Programming with Java: “Chapter 2: Search”**
    Link: Mark Watson’s *Practical Artificial Intelligence Programming
    with Java*: ["Chapter 2:
    Search"](http://www.saylor.org/site/wp-content/uploads/2011/11/CS405-1.1-WATSON.pdf)
    (PDF)  
        
     Instructions: Select the above link and read chapter 2, page 5, up
    to section 2.1.  This introduces the search problem.  One way to
    solve a problem is by searching for a solution in a set, called the
    search space.  This approach assumes that a search can be done in an
    acceptable amount of time at an acceptable cost.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-NoDerivs Unported License
    3.0](http://creativecommons.org/licenses/by-nc-nd/3.0/) (HTML).  It
    is attributed to Mark Watson and the original version can be found
    [here](http://markwatson.com/opencontent/JavaAI3rd.pdf) (PDF).

**2.1.1 Problem Statement** <span id="2.1.1"></span> 
-   **Reading: Mark Watson’s Practical Artificial Intelligence
    Programming with Java: “Chapter 2: Search”**
    Link: Mark Watson’s *Practical Artificial Intelligence Programming
    with Java*: ["Chapter 2:
    Search"](http://www.saylor.org/site/wp-content/uploads/2011/11/CS405-1.1-WATSON.pdf)
    (PDF)  
        
     Instructions: Select the link above and read chapter 2, section
    2.1, which introduces a tree representation for a search space.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-NoDerivs Unported License
    3.0](http://creativecommons.org/licenses/by-nc-nd/3.0/) (HTML).  It
    is attributed to Mark Watson and the original version can be found
    [here](http://markwatson.com/opencontent/JavaAI3rd.pdf) (PDF).

**2.1.2 Terminology and Definitions** <span id="2.1.2"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 2: Search1”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: ["Chapter 2:
    Search1"](http://www.saylor.org/site/wp-content/uploads/2011/11/CS405-2.1.2-MIT.pdf)
    (PDF)  
        
     Instructions: Study the first 10 slides, slides 2.1.1 to 2.1.10, in
    section 6.034 Notes: Section 2.1, on the use of trees and graphs for
    the representation of search state spaces.  These slides present
    terminology for trees and graphs.   
        
     This reading applies to 2.1.2.1 through 2.1.2.3 below.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF). 

**2.1.2.1 Trees and Nodes** <span id="2.1.2.1"></span> 
*Note: This subunit is covered by the MIT reading assigned in subunit
2.1.2, slides 1 and 2, which introduce search of trees and graphs as a
basic problem-solving approach.*

**2.1.2.2 Graphs** <span id="2.1.2.2"></span> 
*Note: This subunit is covered by the MIT reading assigned in subunit
2.1.2, slides 1 and 2.  A graph is a tree that may contain loops and
multiple parent nodes.  We are interested in graphs where the links have
direction.*

**2.1.2.2.1 Directed** <span id="2.1.2.2.1"></span> 
*Note: This subunit is covered by the MIT reading assigned in 2.1.2
above, slide 3.  A directed graph is a graph where the links have
direction—like a one-way street.*

**2.1.2.2.2 Undirected** <span id="2.1.2.2.2"></span> 
*Note: This subunit is covered by the MIT reading assigned in 2.1.2
above, slide 4.  An undirected graph is defined here as a graph where
the links go in both directions—like a two-way street.  Examples of
graphs are given in slides 5–6.*

**2.1.2.3 States, Actions, and Goals** <span id="2.1.2.3"></span> 
*Note: This subunit is covered by the MIT reading of 2.1.2 above, slides
7–10.  These slides describe the use of trees and graphs in solving
problems using search.  They show how graph searching can be transformed
into tree searching and how trees can be used to model problems by using
nodes to represent states, links to represent actions, and specific
nodes to represent goals.  *

**2.2 Types of Searches** <span id="2.2"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 2: Search1”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: ["Chapter 2:
    Search1"](http://www.saylor.org/site/wp-content/uploads/2011/11/CS405-2.1.2-MIT.pdf) (PDF)  
                              
     Instructions: Study slides 2.2.1 to 2.2.6 in section 6.034 Notes:
    Section 2.2, on searching trees and graphs for a path.  Four classes
    of searches are described, along with ways to implement them.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF).   

**2.2.1 Any Path, Uninformed** <span id="2.2.1"></span> 
-   **Reading: Mark Watson’s Practical Artificial Intelligence
    Programming with Java: “Chapter 2: Search”**
    Link: Mark Watson’s *Practical Artificial Intelligence Programming
    with Java*: ["Chapter 2:
    Search"](http://www.saylor.org/site/wp-content/uploads/2011/11/CS405-1.1-WATSON.pdf)
    (PDF)           
        
     Instructions: Select the link above and read sections 2.2 and 2.3
    for ideas on basic searching and implementing the ideas in Java
    programs.  These ideas are expanded upon in the lecture readings
    below.  This reading also applies to 2.2.1.1 and 2.2.1.2.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-NoDerivs Unported License
    3.0](http://creativecommons.org/licenses/by-nc-nd/3.0/) (HTML).  It
    is attributed to Mark Watson and the original version can be found
    [here](http://markwatson.com/opencontent/JavaAI3rd.pdf) (PDF).

-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 2: Search1”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: ["Chapter 2”
    Search1"](http://www.saylor.org/site/wp-content/uploads/2011/11/CS405-2.1.2-MIT.pdf)
    (PDF)  
        
     Instructions: Study slides 2.2.7 through 2.2.18 for implementation
    guidance for Depth-First and Breadth-First searches, including the
    use of heuristics to improve the efficiency of the search.  Slides
    2.2.19 to 2.2.29 discuss the performance of the Depth-First and
    Breadth-First algorithms with respect to time and space (memory). 
    Read slides 2.3.1–2.3.13 that step through the Depth-First search
    algorithm.  Also, read slides 2.3.14–2.3.24, which step through the
    Breadth-First search algorithm.  Stepping through the algorithms
    shows what happens when they are executing; this insight leads to an
    improved algorithm, called Progressive Deepening.   
        
     These readings also apply to sections 2.2.1.1 and 2.2.1.2.  Slides
    2.2.15–2.2.18 apply to 2.2.2.2 below.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF). 

**2.2.1.1 Depth-First** <span id="2.2.1.1"></span> 
*Note: This subunit is covered by the MIT reading of 2.2.1 above.  In
Depth-First Search, the search traverses along the links to descendants,
to a particular depth, before traversing the links to siblings.*

**2.2.1.2 Breadth-First** <span id="2.2.1.2"></span> 
*Note: This subunit is covered by the MIT reading of 2.2.1 above.  In
Breadth-First Search, the search traverses along the links to siblings
before traversing the links to descendants. *

**2.2.2 Any Path, Informed** <span id="2.2.2"></span> 
-   **Reading: Mark Watson’s Practical Artificial Intelligence
    Programming with Java: “Chapter 2: Search”**
    Link: Mark Watson’s *Practical Artificial Intelligence Programming
    with Java*: ["Chapter 2:
    Search"](http://www.saylor.org/site/wp-content/uploads/2011/11/CS405-1.1-WATSON.pdf) (PDF)  
         
     Instructions: Select the link above and read section 2.4 for ideas
    on improving searching and implementing the ideas in Java programs. 
    These ideas are expanded upon in the readings below.  This reading
    also applies to 2.2.2.1 and 2.2.2.2.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-NoDerivs Unported License
    3.0](http://creativecommons.org/licenses/by-nc-nd/3.0/) (HTML).  It
    is attributed to Mark Watson and the original version can be found
    [here](http://markwatson.com/opencontent/JavaAI3rd.pdf) (PDF).

-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 2: Search1”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: ["Chapter 2:
    Search1"](http://www.saylor.org/site/wp-content/uploads/2011/11/CS405-2.1.2-MIT.pdf)
    (PDF)  
        
     Instructions: Study slides 2.2.30 through 2.2.36, which show that
    combining the Depth-First and Breadth-First strategies gives better
    performance with respect to time and space.  Read slides
    2.3.25–2.3.31, which step through the Best-First search algorithm,
    which utilizes a heuristic value in selecting the next node to
    search.   
        
     This reading also applies to 2.2.2.1 and 2.2.2.2.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF). 

**2.2.2.1 Best-First** <span id="2.2.2.1"></span> 
*Note: This subunit is covered by the MIT reading of 2.2.2 above. 
Depth-First and Breadth-First are called 'blind' searches or uninformed
searches.  Best-First uses a heuristic value of the nodes to select
which link to traverse next.  It selects the link that goes to the node
with the best heuristic value.  Searches that use information about the
problem goal to select nodes to traverse to are called heuristic
searches, or informed searches. *

**2.2.2.2 Heuristics** <span id="2.2.2.2"></span> 
*Note: This subunit is covered by the MIT reading of 2.2.1 above, slides
2.2.15–2.2.18.  Also, this subunit is addressed by the MIT reading of
2.2.2, slide 2.3.25.*

**2.2.3 Optimal, Uninformed** <span id="2.2.3"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 2: Search2”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: ["Chapter 2:
    Search2"](http://www.saylor.org/site/wp-content/uploads/2011/11/CS405-2.2.3-MIT.pdf)
    (PDF)  
        
     Instructions: Study slides 2.4.1–2.4.34 in 6.034 Notes: Section
    2.4, on the uniform cost algorithm, which finds the shortest
    path.   
        
     These slides apply to sections 2.2.3.1 and 2.2.3.2 below.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF).

**2.2.3.1 Uniform Cost** <span id="2.2.3.1"></span> 
*Note: This subunit is covered by the MIT reading of 2.2.3 above.  The
Uniform Cost search algorithm is an optimal, uninformed search.  Each
link has an associated cost.  The cost of a path is the sum of the cost
of the links that comprise the path.  The Uniform Cost algorithm selects
and expands the node that has the lowest cost.*

**2.2.3.2 Shortest Path** <span id="2.2.3.2"></span> 
*Note: This subunit is covered by the MIT reading of 2.2.3 above.  If
the cost of a link is the distance between the end nodes of the link,
then the Uniform Cost Algorithm finds the shortest path from the start
node to the goal node. The Uniform Cost Algorithm uses the “past”
information, i.e., information about a path from the start node to a
node, instead of information about a path from a node to the goal node.*

**2.2.4 Optimal, Informed** <span id="2.2.4"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 2: Search2”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: ["Chapter 2:
    Search2"](http://www.saylor.org/site/wp-content/uploads/2011/11/CS405-2.2.3-MIT.pdf)
    (PDF)  
        
     Instructions: Study slides 2.5.1– 2.5.21, in 6.034 Notes: Section
    2.5, on the A\* algorithm, which finds the shortest path to a goal
    (an optimal path) using a heuristic estimate of the distance to the
    goal.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF). 

**2.2.4.1 A\*** <span id="2.2.4.1"></span> 
*Note: This subunit is covered by the MIT reading of 2.2.4.  Uniform
Cost that uses the estimated total cost of a path from the start node to
the goal (which is the sum of the cost from the start to a node + the
estimated cost from the node to the goal) is called an A\* algorithm.  *

**2.2.4.2 Heuristic Shortest Path** <span id="2.2.4.2"></span> 
*Note: This subunit is covered by the MIT reading of 2.2.4.  When the
A\* algorithm uses distance or length for the associated cost of a link,
then the A\* algorithm finds the shortest path using the estimated total
distance from the start node to the goal as the heuristic.  *

**2.3 Time and Space Requirements, More on Heuristics and Complexity**
<span id="2.3"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 2: Search1”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: ["Chapter 2:
    Search1"](http://www.saylor.org/site/wp-content/uploads/2011/11/CS405-2.1.2-MIT.pdf)
    (PDF)  
        
     Instructions: Read slides 2.2.19 to 2.2.31, in the PDF file Chapter
    2: Search1, section 6.034 Notes: Section 2.2, about the efficiency
    of the four types of searches.  Efficiency considers time, cost, and
    resources, such as memory.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF). 

-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 2: Search3”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: ["Chapter 2:
    Search3"](http://www.saylor.org/site/wp-content/uploads/2011/11/CS405-2.3-MIT.pdf)
    (PDF)  
        
     Instructions: Read slides 2.6.1 to 2.7.26, in the PDF file Chapter
    2: Search3, section 6.034 Notes: Sections 2.6 and 2.7, for
    additional information on heuristics for optimality (finding an
    optimal path to a goal), and about complexity and efficiency of
    search.  Efficiency considers time, cost, and resources, such as
    memory.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF). 


