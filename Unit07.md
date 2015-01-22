**Unit 7: Natural Language Understanding** <span id="7"></span> 
*This unit will provide you with a basic introduction to Natural
Language Understanding (NLU) in AI.  Syntax, semantics, and ambiguity of
natural language are discussed.  Simple examples are presented.  Some of
what we have seen, in search and in learning, is applied in NLU. 
Natural language processing and understanding is a large field of
research and has entire courses devoted to it.  So, in this
introduction, our objective is simply to introduce the problems and
approaches.*

**Unit 7 Time Advisory**  
This unit should take approximately 20 hours to complete.  
  
 ☐    Subunit 7.1: 6 hours plus 2 hours video
  
 ☐    Subunit 7.1.1: 2 hours  
  
 ☐    <span class="Apple-style-span"
style="text-align: -webkit-auto; ">Subunit 7.1.2: 2 hours</span>  
  
 ☐    <span class="Apple-style-span"
style="text-align: -webkit-auto; ">Subunit 7.1.3: 2 hours</span>

☐    Subunit 7.2: 4 hours  
  
 ☐    Subunit 7.3: 7 plus 1-hour video
  
 ☐    Subunit 7.3.1: 1 hour  
  
 ☐    <span class="Apple-style-span"
style="text-align: -webkit-auto; ">Subunit 7.3.2: 1 hour</span>  
  
 ☐    <span class="Apple-style-span"
style="text-align: -webkit-auto; ">Subunit 7.3.3: 1 hour</span>  
  
 ☐    <span class="Apple-style-span"
style="text-align: -webkit-auto; ">Subunit 7.3.4: 1 hour</span>  
  
 ☐    <span class="Apple-style-span"
style="text-align: -webkit-auto; ">Subunit 7.3.5: 3 hours</span>

**Unit7 Learning Outcomes**  
Upon successful completion of this unit, the student will be able to:  
  
-   Describe the progress and applications of natural language
    understanding.
-   Describe the syntax and semantics of natural language.
-   Explain and give examples of the challenges of natural language
    understanding.

**7.1 Language Overview and Basics** <span id="7.1"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 12: Language Understanding”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: ["Chapter 12: Language
    Understanding"](http://www.saylor.org/site/wp-content/uploads/2011/11/CS405-7.1-MIT.pdf)
    (PDF)  
        
     Instructions: Read slides 12.1.1–12.1.7, in 6.034 Notes: Section
    12.1, on an architecture for understanding natural language. 
    Understanding is connecting a natural language sentence to knowledge
    about the world.   
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF).

-   **Lecture: Stanford University: Manning CS224N Natural Language
    Processing Course: “Lecture 1”**
    Link: Stanford University: Manning CS224N Natural Language
    Processing Course: “[Lecture
    1](http://see.stanford.edu/see/lecturelist.aspx?coll=63480b48-8819-4efd-8412-263f1a472f5a)”
    (Silverlight)  
        
     Instructions: Select the link and scroll to Lecture 1.  Watch the
    video lecture by Professor Manning, which introduces the problem of
    natural language processing and understanding.  
        
     Terms of Use: Please respect the copyright and terms of use
    displayed on the webpages above.

**7.1.1 Language Analysis: Syntax and Grammars** <span
id="7.1.1"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 12: Language Understanding”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: ["Chapter 12: Language
    Understanding"](http://www.saylor.org/site/wp-content/uploads/2011/11/CS405-7.1-MIT.pdf)
    (PDF)  
        
     Instructions: Read slides 12.1.1–12.1.7, in 6.034 Notes: Section
    12.1, on the different types of grammars.  Natural language is not
    context free, but a practical approach to NLU can still be made
    using context free languages, because they can express a lot of the
    structure of natural language.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF).

**7.1.2 Parsing: Top-Down, Forward Chaining, Bottom-Up** <span
id="7.1.2"></span> 
-   **Lecture: Stanford University: Manning CS224N Natural Language
    Processing Course: “Lecture 10”**
    Link: Stanford University: Manning CS224N Natural Language
    Processing Course: “[Lecture
    10](http://see.stanford.edu/see/lecturelist.aspx?coll=63480b48-8819-4efd-8412-263f1a472f5a)”
    (Silverlight)  
        
     Instructions: Select the link and scroll down to Lecture 10.  Watch
    the video lecture by Professor Manning, which discusses parsing.  
        
     Terms of Use: Please respect the copyright and terms of use
    displayed on the webpages above.

-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 12: Language Understanding”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: ["Chapter 12: Language
    Understanding"](http://www.saylor.org/site/wp-content/uploads/2011/11/CS405-7.1-MIT.pdf)
    (PDF)  
        
     Instructions: Read slides 12.1.7–12.1.55, in 6.034 Notes: Section
    12.1, on parsing, i.e., finding the structure of a sentence in terms
    of the grammar of the language.   
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF).

**7.1.3 Ambiguity** <span id="7.1.3"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 12: Language Understanding”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: ["Chapter 12: Language
    Understanding"](http://www.saylor.org/site/wp-content/uploads/2011/11/CS405-7.1-MIT.pdf)
    (PDF)  
        
     Instructions: Read slides 12.1.56–12.1.61 in 6.034 Notes: Section
    12.1, on lexical and attachment ambiguity.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF).

**7.2 Syntax Details** <span id="7.2"></span> 
**7.2.1 Constraints** <span id="7.2.1"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 12: Language Understanding”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: "[Chapter 12: Language
    Understanding](http://www.saylor.org/site/wp-content/uploads/2011/11/CS405-7.1-MIT.pdf)”
    (PDF)  
        
     Instructions: Read slides 12.2.1–12.2.9, in 6.034 Notes: Section
    12.2, on constraints, e.g., subjects must agree with verbs and verbs
    must agree with their objects.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF).

**7.2.2 Sub-Categorization** <span id="7.2.2"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 12: Language Understanding”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: ["Chapter 12: Language
    Understanding"](http://www.saylor.org/site/wp-content/uploads/2011/11/CS405-7.1-MIT.pdf)
    (PDF)  
        
     Instructions: Read slides 12.2.10–12.2.19, in 6.034 Notes: Section
    12.2, on the use of recursive rules to handle constraints on
    verbs.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF).

**7.2.3 Grammar Gaps** <span id="7.2.3"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 12: Language Understanding”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: ["Chapter 12: Language
    Understanding"](http://www.saylor.org/site/wp-content/uploads/2011/11/CS405-7.1-MIT.pdf)
    (PDF)  
        
     Instructions: Read slides 12.2.19–12.2.50, in 6.034 Notes: Section
    12.2, on dependencies that are far apart.  These are called gaps. 
    Remember that the NLU wants to capture the meaning, including
    relationships.  If a relative clause occurs, it refers to some
    person mentioned earlier or later.  This reference is called a
    gap.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF).                       

**7.3 Semantic Details** <span id="7.3"></span> 
-   **Lecture: Stanford University: Manning CS224N Natural Language
    Processing Course: “Lecture 12”**
    Link: Stanford University: Manning CS224N Natural Language
    Processing Course: “[Lecture
    12](http://see.stanford.edu/see/lecturelist.aspx?coll=63480b48-8819-4efd-8412-263f1a472f5a)”
    (Silverlight)  
        
     Instructions: Select the link and scroll down to Lecture 12.  Watch
    the guest video lecture by Professor Jurafsky, which talks about
    semantics.  
        
     Terms of Use: Please respect the copyright and terms of use
    displayed on the webpages above.

**7.3.1 From Syntactic Structure to Semantic Structure in Logic** <span
id="7.3.1"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 12: Language Understanding II”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: ["Chapter 12: Language Understanding
    II"](http://www.saylor.org/site/wp-content/uploads/2011/11/CS405-7.3.1-MIT.pdf)
    (PDF)  
        
     Instructions: Read slides 12.3.1–12.3.6, in 6.034 Notes: Section
    12.3, which address obtaining meaning just from the syntax of a
    sentence; use of context information to add to the meaning will come
    later.  (Recall the steps of the NLU architecture.)  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF).

**7.3.2 Composing Semantics** <span id="7.3.2"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 12: Language Understanding II”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: ["Chapter 12: Language Understanding
    II"](http://www.saylor.org/site/wp-content/uploads/2011/11/CS405-7.3.1-MIT.pdf)
    (PDF)  
        
     Instructions: Read slides 12.3.7–12.3.12, in 6.034 Notes: Section
    12.3, on using the semantics of constituent parts of a sentence to
    obtain the semantics of the sentence they compose.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF).

**7.3.3 Quantifiers** <span id="7.3.3"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 12: Language Understanding II”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: ["Chapter 12: Language Understanding
    II"](http://www.saylor.org/site/wp-content/uploads/2011/11/CS405-7.3.1-MIT.pdf)
    (PDF)  
        
     Instructions: Read slides 12.3.13–12.3.23, in 6.034 Notes: Section
    12.3, on the semantics of quantifiers.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF).

**7.3.4 Ambiguity** <span id="7.3.4"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 12: Language Understanding II”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: ["Chapter 12: Language Understanding
    II"](http://www.saylor.org/site/wp-content/uploads/2011/11/CS405-7.3.1-MIT.pdf)
    (PDF)  
        
     Instructions: Read slides 12.3.24–12.3.28, in 6.034 Notes: Section
    12.3, which address the next step in the NLU architecture, namely,
    the use of context to resolve ambiguity.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF).

**7.3.5 Simple Language Examples** <span id="7.3.5"></span> 
**7.3.5.1 Database Example** <span id="7.3.5.1"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 12: Language Understanding II”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: ["Chapter 12: Language Understanding
    II"](http://www.saylor.org/site/wp-content/uploads/2011/11/CS405-7.3.1-MIT.pdf)
    (PDF)  
        
     Instructions: Read slides 12.3.29–12.3.48, in 6.034 Notes: Section
    12.3, on application of the NLU processing to a genealogy database
    system.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF).

**7.3.5.2 Programming NL Applications** <span id="7.3.5.2"></span> 
-   **Reading: Mark Watson’s Practical Artificial Intelligence
    Programming with Java: “Chapter 9: Statistical Natural Language
    Processing”**
    Link: Mark Watson’s *Practical Artificial Intelligence Programming
    with Java*: [Chapter 9: Statistical Natural Language
    Processing](http://www.saylor.org/site/wp-content/uploads/2011/11/CS405-1.1-WATSON.pdf) (PDF)  
        
     Instructions: Select the above link and read chapter 9, pages
    137–176, which gives a lot of practical examples of NLP from a
    programming perspective.  In addition, read chapter 10, the next
    chapter, using this same link, but pages 177–206, which provides
    additional discussion on extracting semantic information from text
    and databases.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-NoDerivs Unported License
    3.0](http://creativecommons.org/licenses/by-nc-nd/3.0/) (HTML).  It
    is attributed to Mark Watson and the original version can be found
    [here](http://markwatson.com/opencontent/JavaAI3rd.pdf) (PDF). 

**7.3.5.3 Information** <span id="7.3.5.3"></span> 
-   **Reading: Mark Watson’s Practical Artificial Intelligence
    Programming with Java: “Chapter: 10 Information Gathering”**
    Link: Mark Watson’s Practical Artificial Intelligence Programming
    with Java: “[Chapter 10: Information
    Gathering](http://www.saylor.org/site/wp-content/uploads/2011/11/CS405-1.1-WATSON.pdf)”
    (PDF)  
        
     Instructions: Select the above link and read chapter 10, pages
    177–205, which describes information extraction and discovery.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-NoDerivs Unported License
    3.0](http://creativecommons.org/licenses/by-nc-nd/3.0/) (HTML).  It
    is attributed to Mark Watson and the original version can be found
    [here](http://markwatson.com/opencontent/JavaAI3rd.pdf) (PDF). 


