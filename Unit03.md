---
layout: default
title: "CS405: Artificial Intelligence"
course_description: "An introduction to the fundamental concepts and techniques of intelligent systems. Explores state-space and problem-induction representations of problems, heuristic methods, and how these methods can be applied to artificial intelligence problems."
next: ../Unit04
previous: ../Unit02
---
**Unit 3: Constraint Satisfaction** <span id="3"></span> 
*AI applications are built upon the idea of a problem statement with
constraints.  In AI, we must work within those constraints in order to
develop an optimal solution.  In this unit, we will define “problem” in
specific AI terms and discuss different approaches to constraint
satisfaction.  Constraint satisfaction is an important subject area
within AI.  The famous Map Coloring Problem has simple variables and
simple constraints and is thus useful in illustrating the basics of
constraint satisfaction.  By the end of this unit, you will be able to
solve basic problems.*

**Unit 3 Time Advisory**  
This unit should take approximately 10 hours to complete.  
  
 ☐    Subunit 3.1: 2 hours  
  
 ☐    Subunit 3.2: 8 hours
  
 ☐    Subunit 3.2.1: 2 hours  
  
 ☐    <span class="Apple-style-span"
style="text-align: -webkit-auto; ">Subunit 3.2.2: 2 hours</span>  
  
 ☐    <span class="Apple-style-span"
style="text-align: -webkit-auto; ">Subunit 3.2.3: 2 hours</span>  
  
 ☐    <span class="Apple-style-span"
style="text-align: -webkit-auto; ">Subunit 3.2.4: 2 hours</span>

**Unit3 Learning Outcomes**  
Upon successful completion of this unit, the student will be able to:  
  
-   Apply constraint satisfaction to techniques in solving problems, in
    particular using searching.
-   Describe several heuristics used in constraint satisfaction.

**3.1 Problem Definition** <span id="3.1"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 3: Constraint Satisfactory Problems
    (CSP) and Games1”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: "[Chapter 3: Constraint Satisfactory Problems (CSP) and
    Games1](https://resources.saylor.org/wwwresources/archived/site/wp-content/uploads/2011/11/CS405-3.1-MIT.pdf)”
    (PDF)  
        
     Instructions: Study slides 3.1.1–3.1.19 in 6.034 Notes: Section:
    3.1.  CSP stands for Constraint Satisfaction Problems, which
    include, for example, problems in task scheduling, planning robot
    actions, solving puzzles (for example, the classic N-Queens Problem
    and the Four Color Problem), and interpreting sensory data.  This
    reading applies to sections 3.1.1–3.1.3 below.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF).

**3.1.1 Variable Domains and Constraints** <span id="3.1.1"></span> 
*Note: This subunit is covered by the MIT reading of 3.1.  See slides
3.1.1 and 3.1.13–3.1.15.  *

**3.1.2 Constraint Graph** <span id="3.1.2"></span> 
*Note: This subunit is covered by the MIT reading of 3.1.  See slides
3.1.2 and 3.1.16–3.1.19. *

**3.1.3 Goal: Assign Variable Values Based on Stated Constraints** <span
id="3.1.3"></span> 
*Note: This subunit is covered by the MIT reading of 3.1.  See slide
3.1.2.*

**3.2 Problem Approaches** <span id="3.2"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 3: Constraint Satisfactory Problems
    (CSP) and Games1”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: "[Chapter 3: Constraint Satisfactory Problems (CSP) and
    Games1](https://resources.saylor.org/wwwresources/archived/site/wp-content/uploads/2011/11/CS405-3.1-MIT.pdf)”
    (PDF)  
        
     Instructions: Study slides 3.2.1–3.2.37 in 6.034 Notes: Section
    3.2, on constraint problems and solving them using searching with
    backtracking and forward checking.  This reading applies to sections
    3.2.1–3.2.3 below.  Section 3 in the 6.034 Notes gives another
    improvement—dynamic ordering.   
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF).

**3.2.1 Constraint Propagation (Arc Consistency)** <span
id="3.2.1"></span> 
*Note: This subunit is covered by the MIT reading of 3.2.  See slides
3.2.*1–3.2.16.

**3.2.2 Backtracking** <span id="3.2.2"></span> 
*Note: This subunit is covered by the MIT reading of 3.2.  See slides
3.2.17–3.2.24.*

**3.2.3 Forward Checking** <span id="3.2.3"></span> 
*Note: This subunit is covered by the MIT reading of 3.2.  See slides
3.2.24–3.2.37.*

**3.2.4 Heuristics** <span id="3.2.4"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 3: Constraint Satisfactory Problems
    (CSP) and Games1”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: "[Chapter 3: Constraint Satisfactory Problems (CSP) and
    Games1](https://resources.saylor.org/wwwresources/archived/site/wp-content/uploads/2011/11/CS405-3.1-MIT.pdf)”
    (PDF)  
        
     Instructions: Open the PDF and study Section 3.3, slides
    3.3.1–3.3.12.  This reading also applies to 3.2.4.1 and 3.2.4.2
    below.   
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF).

**3.2.4.1 Dynamic Ordering** <span id="3.2.4.1"></span> 
*Note: This subunit is covered by the MIT reading of 3.2.4.  See slides
3.3.1–3.3.7.  This approach makes the search more efficient by
reordering the variables using information available during the search.*

**3.2.4.2 Incremental Repair** <span id="3.2.4.2"></span> 
*Note: This subunit is covered by the MIT reading of 3.2.4.  See slides
3.3.7–3.3.12.  Incremental repair is another heuristic approach to
making the search more efficient.  It can be done without backtracking
or used in conjunction with backtracking. *


