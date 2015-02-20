---
layout: default
title: "CS405: Artificial Intelligence"
course_description: "An introduction to the fundamental concepts and techniques of intelligent systems. Explores state-space and problem-induction representations of problems, heuristic methods, and how these methods can be applied to artificial intelligence problems."
next: ../Unit06
previous: ../Unit04
---
**Unit 5: Logic** <span id="5"></span> 
*We have already briefly discussed logic, but this unit will provide you
with a more formal definition.  We will learn about two main types of
logic—propositional and first-order.  Prolog was designed for expressing
logic.  This unit gives you a strong foundation in logic so that you
will be able to use or learn Prolog more easily to program logic
applications.  Similarly, you will be able to use or learn class
libraries that support AI techniques in other languages, like C++ and
Java.*

**Unit 5 Time Advisory**  
This unit should take approximately 24 hours to complete.  
  
 ☐    Subunit 5.1: 1 hour  
  
 ☐    Subunit 5.2: 19 hours
  
 ☐    Subunit 5.2.1: 6 hours  
  
 ☐    <span class="Apple-style-span"
style="text-align: -webkit-auto; ">Subunit 5.2.2: 13 hours</span>

☐    Subunit 5.2.2.1: 1 hour  
  
 ☐    <span class="Apple-style-span"
style="text-align: -webkit-auto; ">Subunit 5.2.2.2: 2 hours</span>  
  
 ☐    <span class="Apple-style-span"
style="text-align: -webkit-auto; ">Subunit 5.2.2.3: 3 hours</span>  
  
 ☐    <span class="Apple-style-span"
style="text-align: -webkit-auto; ">Subunit 5.2.2.4: 3 hours</span>  
  
 ☐    <span class="Apple-style-span"
style="text-align: -webkit-auto; ">Subunit 5.2.2.5: 4 hours</span>

☐    Subunit 5.3: 4 hours

**Unit5 Learning Outcomes**  
Upon successful completion of this unit, the student will be able to:  
  
-   Explain the syntax and semantics of logic statements.
-   Write statements, operate on statements, apply the rules of logic to
    transform a statement to equivalent statements, and evaluate
    statements in both the propositional and predicate calculus.
-   Make inferences and prove statements in logic.

**5.1 Definition of Logic** <span id="5.1"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 9: Logic I”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: ["Chapter 9: Logic
    I"](http://www.saylor.org/site/wp-content/uploads/2011/11/CS405-5.1-MIT.pdf) (PDF)  
        
     Instructions: Study slides 9.1.1–9.1.7, in 6.034 Notes: Section
    9.1, which define a logic system as a formal language having syntax,
    semantics, and a proof system.   
        
     This reading applies to subsections 5.1.1–5.1.3.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF).

**5.1.1 Formal Language** <span id="5.1.1"></span> 
*Note: The reading of 5.1 applies to this subunit.  See slide 9.1.1. 
Logic is a formal language and the definitions, rules, and techniques
that are used for formal languages apply to logic statements. *

**5.1.2 Building Blocks, Syntax, and Semantics** <span
id="5.1.2"></span> 
*Note: The reading of 5.1 applies to this subunit.  As with formal
languages, logic statements have syntax—rules for writing well-formed
statements in logic.  Statements also have semantics, which describes
the meaning associated with the statement.  The meaning derives from
associations of the elements of the logic statement with elements of a
domain of discourse.  From this association, the truth or falsehood of a
statement can be determined.  (A domain of discourse is a set of
members, with rules for making assertions about the members, wherein the
truth or falsehood of assertions is known or can be inferred*.)

**5.1.3 Relation to Proof Systems** <span id="5.1.3"></span> 
-   **Reading: UCI: Max Welling’s ICS 171 Introduction to Artificial
    Intelligence Course: “Slides Lecture 8 (Logic 2)”**
    Link: UCI: Max Welling’s ICS 171 Introduction to Artificial
    Intelligence Course: “[Slides Lecture 8 (Logic
    2)](http://www.ics.uci.edu/~welling/teaching/ICS171spring07/ICS171spring07.html)”
    (PPT)  
        
     Instructions: Select the PowerPoint file slides lecture 8 (Logic 2)
    and read the slides 1–4.  These will be elaborated in later sections
    covering the propositional calculus and the predicate calculus.  
        
     Terms of Use: Please respect the copyright and terms of use
    displayed on the webpages above.

**5.2 Types of Logic** <span id="5.2"></span> 
*Note: We will be using two types of logic: propositional logic and
first-order logic.  The difference between the two is in the use of
variables.  Propositional logic has no variables that take on values in
a domain.  For example, P is a sentence in the proposition calculus that
is true or false.  An example for the predicate calculus is P(X,Y),
where P is a relation and X and Y are variables that take on values in a
domain of discourse.  The predicate calculus, also called the
first-order calculus, extends the propositional calculus. *

**5.2.1 Propositional Logic** <span id="5.2.1"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 9: Logic I”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: ["Chapter 9: Logic
    I"](http://www.saylor.org/site/wp-content/uploads/2011/11/CS405-5.1-MIT.pdf)
    (PDF)  
        
     Instructions: Study slides 9.1.8–9.1.16, in 6.034 Notes: Section
    9.1, which define the propositional logic syntax.  This reading
    applies to subsections 5.2.1.1 and 5.2.1.2.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF).

**5.2.1.1 Syntax and Well-Formed Formulas (Sentences)** <span
id="5.2.1.1"></span> 
*Note: The readings of 5.2.1 apply to this subunit.  Slides 9.1.8–9.1.15
describe the syntax and how to write well-formed formulas (wffs) or
legal sentences in the propositional calculus. *

**5.2.1.2 Order of Operations** <span id="5.2.1.2"></span> 
*Note: The readings of 5.2.1 apply to this subunit also.  Slide 9.1.16
gives the order in which operators are applied to wffs. *

**5.2.1.3 Interpretation and “Meaning,” or Semantics, of a Sentence**
<span id="5.2.1.3"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 9: Logic I”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: ["Chapter 9: Logic
    I"](http://www.saylor.org/site/wp-content/uploads/2011/11/CS405-5.1-MIT.pdf) (PDF)  
        
     Instructions: Study slides 9.2.1–9.2.16, in 6.034 Notes: Section
    9.2, which explains semantics, i.e., the meaning of sentences in a
    logic system, in terms of interpretation and semantic rules.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF).

**5.2.1.4 Terminology of “Truth,” and Examples** <span
id="5.2.1.4"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 9: Logic I”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: ["Chapter 9: Logic
    I"](http://www.saylor.org/site/wp-content/uploads/2011/11/CS405-5.1-MIT.pdf)
    (PDF)  
        
     Instructions: Study slides 9.2.17 to 9.2.33, in 6.034 Notes:
    Section 9.2, which define the concepts of validity and
    satisfiability.  These pertain to the “extent” of trueness of a
    sentence.  This reading applies to subsections
    5.2.1.4.1–5.2.1.4.3.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF).

**5.2.1.4.1 Validity** <span id="5.2.1.4.1"></span> 
*Note: The reading of 5.2.1.4 applies to this subunit.  See slide
9.2.18.  Validity is the “strongest” truth, in that a sentence is valid
if it is true for all interpretations. *

**5.2.1.4.2 Satisfiability** <span id="5.2.1.4.2"></span> 
*Note: The reading of 5.2.1.4 applies to this subunit also.  See slide
9.2.19.  A sentence if satisfiable if it is true in some interpretation,
i.e., there is some interpretation for which it is true. *

**5.2.1.4.3 Unsatisfiability** <span id="5.2.1.4.3"></span> 
*Note: The reading of 5.2.1.4 applies to this subunit also.  See slide
9.2.20.  A sentence is unsatisfiable if there is no interpretation for
which it is true, i.e., its value is false for all interpretations.  *

**5.2.1.5 Making Conclusions** <span id="5.2.1.5"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 9: Logic I”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: ["Chapter 9: Logic
    I"](http://www.saylor.org/site/wp-content/uploads/2011/11/CS405-5.1-MIT.pdf)
    (PDF)   
        
     Instructions: Study slides 9.3.1 to 9.3.7, in 6.034 Notes: Section
    9.3, which define the concepts of entailment and proof.  Making a
    conclusion using entailment involves enumerating interpretations,
    which may not be feasible.  Making a conclusion using a proof
    involves applying rules of inference.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF).

**5.2.1.5.1 Entailment** <span id="5.2.1.5.1"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 9: Logic I”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: ["Chapter 9: Logic
    I"](http://www.saylor.org/site/wp-content/uploads/2011/11/CS405-5.1-MIT.pdf)
    (PDF)   
        
     Instructions: Study slides 9.3.8 to 9.3.11 in 6.034 Notes: Section
    9.3.  Entailment is a key concept for understanding the semantics of
    logic and for understanding inference.  It considers sets of
    interpretations.   
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF).

**5.2.1.5.2 Proof** <span id="5.2.1.5.2"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 9: Logic I”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: ["Chapter 9: Logic
    I"](http://www.saylor.org/site/wp-content/uploads/2011/11/CS405-5.1-MIT.pdf)
    (PDF)   
        
     Instructions: Study slides 9.3.12 to 9.3.18, in 6.034 Notes:
    Section 9.3, which discusses proof as a more practical way to draw
    conclusions.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF).

**5.2.1.5.3 Rules of Inference** <span id="5.2.1.5.3"></span> 
**5.2.1.5.3.1 Deduction** <span id="5.2.1.5.3.1"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 9: Logic I”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: ["Chapter 9: Logic
    I"](http://www.saylor.org/site/wp-content/uploads/2011/11/CS405-5.1-MIT.pdf)
    (PDF)   
        
     Instructions: Study slides 9.3.19 to 9.3.34, in 6.034 Notes:
    Section 9.3, which present rules of inference for use in proofs. 
    Slide 9.3.34 presents resolution, a rule of inference amenable to
    programming a proof.  This reading also applies to subsection
    5.2.1.5.3.2.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF).

**5.2.1.5.3.2 Resolution** <span id="5.2.1.5.3.2"></span> 
*Note: This subunit is covered by the reading of 5.2.1.5.3.1. 
Resolution is a deduction technique used in propositional calculus and
also in the predicate calculus, and which was designed for use in
computational applications.  *

**5.2.2 First-Order Logic** <span id="5.2.2"></span> 
**5.2.2.1 Relation to Prepositional Logic and Motivation** <span
id="5.2.2.1"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 9: Logic I”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: ["Chapter 9: Logic
    I"](http://www.saylor.org/site/wp-content/uploads/2011/11/CS405-5.1-MIT.pdf)
    (PDF)   
        
     Instructions: Study slides 9.4.1 to 9.4.7, in 6.034 Notes: Section
    9.4, which present the first-order predicate calculus.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF).

**5.2.2.2 Syntax of First-Order Logic** <span id="5.2.2.2"></span> 
**5.2.2.2.1 Terms** <span id="5.2.2.2.1"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 9: Logic I”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: ["Chapter 9: Logic
    I"](http://www.saylor.org/site/wp-content/uploads/2011/11/CS405-5.1-MIT.pdf)
    (PDF)   
        
     Instructions: Study slides 9.4.7 to 9.4.13, in 6.034 Notes: Section
    9.4, which present the syntax of the first-order predicate calculus
    or, as it is also called, first-order logic.  This reading also
    applies to subsections 5.2.2.2.1.1–5.2.2.2.1.3.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF).

**5.2.2.2.1.1 Constants** <span id="5.2.2.2.1.1"></span> 
*Note: The reading of 5.2.2.2.1 applies to this subunit.  See slides
9.4.8–9.4.11.*   

**5.2.2.2.1.2 Functions** <span id="5.2.2.2.1.2"></span> 
*Note: The reading of 5.2.2.2.1 applies to this subunit.  See slide
9.4.12. *

**5.2.2.2.1.3 Variables and Quantification** <span
id="5.2.2.2.1.3"></span> 
*Note: The reading of 5.2.2.2.1 applies to this subunit.  See slides
9.4.13–9.4.15.*

**5.2.2.2.2 Sentences** <span id="5.2.2.2.2"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 9: Logic I”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: ["Chapter 9: Logic
    I"](http://www.saylor.org/site/wp-content/uploads/2011/11/CS405-5.1-MIT.pdf)
    (PDF)   
        
     Instructions: Study slides 9.4.14 to 9.4.16, in 6.034 Notes:
    Section 9.4, which complete the syntax of the first-order logic. 
    Now we can write terms using constants, variables, and functions. 
    We can write sentences using predicates, and combine predicates and
    sentences to form new sentences using the quantifiers and the
    operators.  This reading also applies to subsections 5.2.2.2.2.1 and
    5.2.2.2.2.2 below.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF).

**5.2.2.2.2.1 Components** <span id="5.2.2.2.2.1"></span> 
*Note: Components are the terms (constants, variables, functions), the
predicates, and the sentences.  The operators apply to sentences and
result in new sentences.*  

**5.2.2.2.2.2 Closure** <span id="5.2.2.2.2.2"></span> 
*Note: The reading of 5.2.2.2.1 applies to this subunit.  See slide
9.4.16.  Closure simply means that when operators are applied to
sentences in the predicate calculus, the result is again a sentence.*

**5.2.2.3 Semantics and Interpretation in First-Order Logic** <span
id="5.2.2.3"></span> 
**5.2.2.3.1 Interpretations** <span id="5.2.2.3.1"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 9: Logic Ib”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: ["Chapter 9: Logic
    Ib"](http://www.saylor.org/site/wp-content/uploads/2011/11/CS405-5.2.2.3.1-MIT.pdf)
    (PDF)   
        
     Instructions: Study slides 9.5.1 to 9.5.8, in 6.034 Notes: Section
    9.5, which define interpretation as three mappings from the constant
    symbols, predicate symbols, and function symbols of an FOL to those
    of a Domain of Discourse.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF).

**5.2.2.3.2 Hold in an Interpretation** <span id="5.2.2.3.2"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 9: Logic Ib”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: ["Chapter 9: Logic
    Ib"](http://www.saylor.org/site/wp-content/uploads/2011/11/CS405-5.2.2.3.1-MIT.pdf)
    (PDF)   
        
     Instructions: Study slides 9.5.9 to 9.5.18, in 6.034 Notes: Section
    9.5.  The slides define the truth of a sentence in an FOL relative
    to an interpretation.  This reading also applies to subsection
    5.2.2.3.3 on the semantics of quantifiers.   
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF).

**5.2.2.3.3 Semantics of Quantifiers** <span id="5.2.2.3.3"></span> 
*Note: The reading of 5.2.2.3.2 applies to this subunit.  For
quantifiers, the variable used in the quantifier is bound to values (or
takes on values) from the interpretation, i.e., values in the domain of
discourse. *

**5.2.2.3.4 Simple-Block-World Example** <span id="5.2.2.3.4"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 9: Logic Ib”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: ["Chapter 9: Logic
    Ib"](http://www.saylor.org/site/wp-content/uploads/2011/11/CS405-5.2.2.3.1-MIT.pdf)
    (PDF)  
        
     Instructions: Study slides 9.5.25 to 9.5.49, in 6.034 Notes:
    Section 9.5.  The slides present an example of a simple block world
    using an FOL.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF).

**5.2.2.4 Representing Real World Problems in FOL** <span
id="5.2.2.4"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 9: Logic Ib”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: "[Chapter 9: Logic
    Ib](http://www.saylor.org/site/wp-content/uploads/2011/11/CS405-5.2.2.3.1-MIT.pdf)”
    (PDF)   
        
     Instructions: Study slides 9.6.1 to 9.6.26, in 6.034 Notes: Section
    9.6, which presents examples of FOL translations of English
    statements.   
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF).

**5.2.2.5 Using FOL to Solve Real World Problems** <span
id="5.2.2.5"></span> 
**5.2.2.5.1 Entailment** <span id="5.2.2.5.1"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 9: Logic Ib”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: ["Chapter 9: Logic
    Ib"](http://www.saylor.org/site/wp-content/uploads/2011/11/CS405-5.2.2.3.1-MIT.pdf)
    (PDF)   
        
     Instructions: Study slides 9.7.1 to 9.7.24, in 6.034 Notes: Section
    9.7, which show that if a knowledge base (KB) entails a sentence,
    then the sentence logically follows from the KB.  However, they also
    show the impracticality of using entailment to prove a conclusion.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF).

**5.2.2.5.2 Proof and Axiomatization** <span id="5.2.2.5.2"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 9: Logic Ib”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: ["Chapter 9: Logic
    Ib"](http://www.saylor.org/site/wp-content/uploads/2011/11/CS405-5.2.2.3.1-MIT.pdf)
    (PDF)   
        
     Instructions: Study slides 9.7.25 to 9.7.43, in 6.034 Notes:
    Section 9.7, which show that a practical way to use FOL to draw
    conclusions from FOL statements is by using proofs.  But in order to
    prove a conclusion the KB needs a set of axioms.  Examples show that
    the axioms have to capture the essential information about a
    domain.  If the axioms are too few, a false conclusion won't be
    proved, but it may not be possible to draw some desired conclusions.
     These slides also apply to the next subsection, 5.2.2.5.3.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF).  

**5.2.2.5.3 Resolution in Propositional Logic and FOL** <span
id="5.2.2.5.3"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 10: Logic II”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: ["Chapter 10: Logic
    II"](http://www.saylor.org/site/wp-content/uploads/2011/11/CS405-5.2.2.5.3-MIT.pdf)
    (PDF)  
        
     Instructions: Read the slides in 6.034 Notes: Section 10.2, on
    reasoning using resolution in propositional logic.  Also, read
    sections 10.3 and 10.4, which deal with FOL.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF).

**5.2.2.5.4 More on FOL Resolution and Examples** <span
id="5.2.2.5.4"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 10: Logic IIb”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: ["Chapter 10: Logic
    IIb"](http://www.saylor.org/site/wp-content/uploads/2011/11/CS405-5.2.2.5.4-MIT.pdf)
    (PDF)  
        
     Instructions: Read the slides, in 6.034 Notes: Sections 10.5 and
    10.6, on FOL resolution, and 10.7 on application examples.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF).

**5.3 Some Examples of Practical Applications** <span id="5.3"></span> 
-   **Reading: Mark Watson’s Practical Artificial Intelligence
    Programming with Java: “Chapter 3: Reasoning”**
    Link: Mark Watson’s *Practical Artificial Intelligence Programming
    with Java*: “[Chapter 3:
    Reasoning](http://www.saylor.org/site/wp-content/uploads/2011/11/CS405-1.1-WATSON.pdf)”
    (PDF)  
        
     Instructions: Select the above link and read chapter 3, pages
    45–56, which gives examples and tools for applying logic.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-NoDerivs Unported License
    3.0](http://creativecommons.org/licenses/by-nc-nd/3.0/) (HTML).  It
    is attributed to Mark Watson and the original version can be found
    [here](http://markwatson.com/opencontent/JavaAI3rd.pdf) (PDF). 

-   **Reading: Mark Watson’s Practical Artificial Intelligence
    Programming with Java: “Chapter 4: Semantic Web”**
    Link: Mark Watson’s *Practical Artificial Intelligence Programming
    with Java*: “[Chapter 4: Semantic
    Web](http://www.saylor.org/site/wp-content/uploads/2011/11/CS405-1.1-WATSON.pdf)”
    (PDF)  
        
     Instructions: Select the above link and read chapter 4, pages
    57–72, which discusses the Semantic Web.  Reasoning assumes a body
    of data from which inferences can be made.  This reading discusses
    the Semantic Web as a source of data for use in programs, in
    particular for inference algorithms.     
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-NoDerivs Unported License
    3.0](http://creativecommons.org/licenses/by-nc-nd/3.0/) (HTML).  It
    is attributed to Mark Watson and the original version can be found
    [here](http://markwatson.com/opencontent/JavaAI3rd.pdf) (PDF). 

-   **Reading: Mark Watson’s Practical Artificial Intelligence
    Programming with Java: “Chapter 5: Expert Systems”**
    Link: Mark Watson’s *Practical Artificial Intelligence Programming
    with Java*: “[Chapter 5: Expert
    Systems](http://www.saylor.org/site/wp-content/uploads/2011/11/CS405-1.1-WATSON.pdf)”(PDF)  
        
     Instructions: Select the above link and read chapter 5, pages
    73–98, which gives examples and tools for expert systems application
    in reasoning.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-NoDerivs Unported License
    3.0](http://creativecommons.org/licenses/by-nc-nd/3.0/) (HTML).  It
    is attributed to Mark Watson and the original version can be found
    [here](http://markwatson.com/opencontent/JavaAI3rd.pdf) (PDF). 


