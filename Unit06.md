---
layout: default
title: "CS405: Artificial Intelligence"
course_description: "An introduction to the fundamental concepts and techniques of intelligent systems. Explores state-space and problem-induction representations of problems, heuristic methods, and how these methods can be applied to artificial intelligence problems."
next: ../Unit07
previous: ../Unit05
---
**Unit 6: Machine Learning** <span id="6"></span> 
*Machine Learning refers to computer programs that are able to
categorize data in order to maximize understanding of that information. 
Machine Learning is closely related to statistics and modeling and has a
wide range of applications, from natural language processing, searching,
robotics, and indexing, to other pattern recognition applications.  This
unit will begin by defining Machine Learning, its applications, and a
number of other important terms that will be used in this unit.  We will
then go over the three main classes of Machine Learning: Supervised
Learning, Semi-Supervised Learning, and Unsupervised Learning.  You will
also end up with an introductory foundation in Machine Learning that
will be useful for further academic study in the field.*

**Unit 6 Time Advisory**  
This unit should take approximately 26 hours to complete.  
  
 ☐    Subunit 6.1: 8 hours
  
 ☐    Subunit 6.1.1: 2 hours  
  
 ☐    <span class="Apple-style-span"
style="text-align: -webkit-auto; ">Subunit 6.1.2: 2 hours</span>  
  
 ☐    <span class="Apple-style-span"
style="text-align: -webkit-auto; ">Subunit 6.1.3: 4 hours</span>

☐    Subunit 6.2: 16 hours
  
 ☐    <span class="Apple-style-span" style="text-align: left; ">Subunit
6.2.1: 5 hours</span>  
  
 ☐    <span class="Apple-style-span"
style="text-align: -webkit-auto; ">Subunit 6.2.2: 4 hours plus 4 hours
video</span>  
  
 ☐    <span class="Apple-style-span"
style="text-align: -webkit-auto; ">Subunit 6.2.3: 3 hours</span>

☐    Subunit 6.3: 2 hours

**Unit6 Learning Outcomes**  
Upon successful completion of this unit, the student will be able to:  
  
-   Define machine learning, the basic concepts and methods used in
    machine learning.
-   Identify the various applications of machine learning.
-   Explain the types of machine learning.
-   Identify the benefits and drawbacks of each type of machine
    learning. 

**6.1 Definition of Learning and Machine Learning** <span
id="6.1"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 4: Learning Introduction”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: ["Chapter 4: Learning
    Introduction"](https://resources.saylor.org/archived/wp-content/uploads/2011/11/CS405-6.1-MIT.pdf)
    (PDF)  
        
     Instructions: Study slides 4.1.1–4.1.7, in 6.034 Notes: Section
    4.1, which introduce the topic of learning.  Machine learning is
    learning using methods that can be implemented in software.  Study
    slides 4.1.8–4.1.31, which are applicable to machine learning.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF).  

**6.1.1 Learning Methods and Problem Set** <span id="6.1.1"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 4: Learning Introduction”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: ["Chapter 4: Learning
    Introduction"](https://resources.saylor.org/archived/wp-content/uploads/2011/11/CS405-6.1-MIT.pdf)
    (PDF)  
        
     Instructions: Study slides 4.1.8–4.1.42, in 6.034 Notes: Section
    4.1, which present learning in terms of learning a function (this is
    called supervised learning when some of the input/output pairs of
    the function are provided—supervised learning will be discussed in a
    later section).  These slides present three learning methods:
    nearest neighbor, decision trees, and neural nets.  Slide 4.1.42
    lists some problems that machine learning has had some success in
    solving.  Slides 4.1.14–4.1.24 give an example of predicting future
    behavior and are applicable to section 6.1.2.2 below.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF).  

**6.1.2 Applications** <span id="6.1.2"></span> 
**6.1.2.1 Data Mining** <span id="6.1.2.1"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 5: Machine Learning I”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: ["Chapter 5: Machine Learning
    I"](https://resources.saylor.org/archived/wp-content/uploads/2011/11/CS405-6.1.2.1-MIT.pdf)
    (PDF)  
        
     Instructions: Read slide 5.1.44, in 6.034 Notes: Section 5.1, on
    data mining.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF)  

**6.1.2.2 Future-Behavior Prediction** <span id="6.1.2.2"></span> 
*Note: See 6.1.1 for applicable slides.  These slides give an example of
predicting a future action by learning from past examples.  *

**6.1.2.3 Genetic Programming** <span id="6.1.2.3"></span> 
-   **Reading: Mark Watson’s Practical Artificial Intelligence
    Programming with Java: “Chapter 6: Genetic Algorithms”**
    Link: Mark Watson’s *Practical Artificial Intelligence Programming
    with Java*: ["Chapter 6: Genetic
    Algorithms"](https://resources.saylor.org/archived/wp-content/uploads/2011/11/CS405-1.1-WATSON.pdf)
    (PDF)  
        
     Instructions: Select the above link and read pages 99–108, where
    you will learn why these algorithms are called genetic.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-NoDerivs Unported License
    3.0](http://creativecommons.org/licenses/by-nc-nd/3.0/) (HTML).  It
    is attributed to Mark Watson and the original version can be found
    [here](http://markwatson.com/opencontent/JavaAI3rd.pdf) (PDF).

**6.1.2.4 Pattern Recognition** <span id="6.1.2.4"></span> 
-   **Reading: Mark Watson’s Practical Artificial Intelligence
    Programming with Java: “Chapter 7: Neural Networks”**
    Link: Mark Watson’s *Practical Artificial Intelligence Programming
    with Java*: ["Chapter 7: Neural
    Networks"](https://resources.saylor.org/archived/wp-content/uploads/2011/11/CS405-1.1-WATSON.pdf)
    (PDF)  
        
     Instructions: Recognition of patterns occurs in search, game
    playing, language recognition, expert systems and rule-based
    systems, vision, and learning.  Select the above link and look over
    chapter 7, section 7.1, Hopfield Neural Networks, pages 110–111,
    where the concept of patterns is utilized in learning in neural
    networks.  
        
     Optional: Browse through the Watson text and look for the use of
    pattern recognition in various applications.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-NoDerivs Unported License
    3.0](http://creativecommons.org/licenses/by-nc-nd/3.0/) (HTML).  It
    is attributed to Mark Watson and the original version can be found
    [here](http://markwatson.com/opencontent/JavaAI3rd.pdf) (PDF).

**6.1.3 Building Blocks** <span id="6.1.3"></span> 
**6.1.3.1 Statistics** <span id="6.1.3.1"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 5: Machine Learning I”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: ["Chapter 5: Machine Learning
    I"](https://resources.saylor.org/archived/wp-content/uploads/2011/11/CS405-6.1.2.1-MIT.pdf)
    (PDF)  
        
     Instructions: Read slides 5.2.30–5.2.39, in 6.034 Notes: Section
    5.2, on Bayes’ rule in probability.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF)  

**6.1.3.2 Features** <span id="6.1.3.2"></span> 
*Note: Features arose in the introduction to clustering on slide 4.1.9
in section 4.1 of ch4\_learnintro.  They come up again in supervised
learning.*

-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 4: Learning Introduction”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: ["Chapter 4: Learning
    Introduction"](https://resources.saylor.org/archived/wp-content/uploads/2011/11/CS405-6.1-MIT.pdf)
    (PDF)  
        
     Instructions: Select the link and study slides 4.2.1–4.2.45, in
    6.034 Notes: Section 4.2, which describe supervised learning using
    features.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF)

-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 10: Feature Spaces”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: ["Chapter 10: Feature
    Spaces"](https://resources.saylor.org/archived/wp-content/uploads/2011/11/CS405-6.1.3.2-MIT.pdf)
    (PDF)  
        
     Instructions: Read slides 10.1.1–10.1.15, in 6.034 Notes: Section
    10.1, on more “complex” features.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF).

-   **Reading: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: “Chapter 8: Machine Learning IV”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: ["Chapter 8: Machine Learning
    IV"](https://resources.saylor.org/archived/wp-content/uploads/2011/11/CS405-6.1.3.2-MIT-PartII.pdf)
    (PDF)  
        
     Instructions: Look over the slides, in 6.034 Notes: Section 8.4. 
    These slides deal with huge numbers of features by feature
    selection, ranking, and applications to clustering.   
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF)

**6.1.3.3 Models** <span id="6.1.3.3"></span> 
*Note: Several models are used in the study of learning, including
decision tree models, probabilistic models such as Bayes’, neuron models
in neural nets, statistical models such as Gaussian distribution models
in classifying data and in building training sets.  These are mentioned
further in their respective sections in 6.2 Types of Machine Learning. *

**6.1.3.4 Data Set** <span id="6.1.3.4"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 4: Learning Introduction”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: ["Chapter 4: Learning
    Introduction"](https://resources.saylor.org/archived/wp-content/uploads/2011/11/CS405-6.1-MIT.pdf)
    (PDF)  
        
     Instructions: Read slides 4.3.1–4.3.43, in 6.034 Notes: Section
    4.3, on test sets, cross-validation, noisy data, and an example
    using Congressional voting.  These slides also apply to subsections
    6.1.3.4.1–6.1.3.4.3.   
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF).

**6.1.3.4.1 Training** <span id="6.1.3.4.1"></span> 
*Note: The reading of 6.1.3.4 applies to this subunit. Learning is based
on training and quality of the training set.*

**6.1.3.4.2 Testing** <span id="6.1.3.4.2"></span> 
*Note: The reading of 6.1.3.4 applies to this subunit.  Testing
determines the quality of the learning that resulted from the
training.* 

**6.1.3.4.3 Validation** <span id="6.1.3.4.3"></span> 
*Note: The reading of 6.1.3.4 applies to this subunit.  Validation
demonstrates that the resulting performance of the learning algorithm
satisfies the objectives of the problem-solving application. *

**6.2 Types of Machine Learning** <span id="6.2"></span> 
**6.2.1 Supervised** <span id="6.2.1"></span> 
**6.2.1.1 Methods** <span id="6.2.1.1"></span> 
**6.2.1.1.1 Decision Trees** <span id="6.2.1.1.1"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 5: Machine Learning I"**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: “[Chapter 5: Machine Learning
    I](https://resources.saylor.org/archived/wp-content/uploads/2011/11/CS405-6.1.2.1-MIT.pdf)”
    (PDF)  
        
     Instructions: Study slides 5.1.1–5.1.44 in 8.034 Section 5.1, on
    decision trees.   
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF).

**6.2.1.1.2 Naive Bayes** <span id="6.2.1.1.2"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 5: Machine Learning I”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: ["Chapter 5: Machine Learning
    I"](https://resources.saylor.org/archived/wp-content/uploads/2011/11/CS405-6.1.2.1-MIT.pdf)
    (PDF)  
        
     Instructions: Read slides 5.2.1–5.2.25, in 6.034 Notes: Section
    5.2, on naïve Bayes inference.  Slides 5.2.26–5.2.29 apply it to an
    example—Congressional voting.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF)

**6.2.1.1.3 Neural Nets** <span id="6.2.1.1.3"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 7: Machine Learning III”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course:["Chapter 7: Machine Learning
    III"](https://resources.saylor.org/archived/wp-content/uploads/2011/11/CS405-6.2.1.1.3-MIT.pdf)
    (PDF)  
        
     Instructions: Read slides 7.3.1–7.3.39, in 6.034 Notes: Section
    7.3, on artificial neural nets. Read slides 7.4.1–7.4.24 in section
    7.4, which discuss training for artificial neural nets.   
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF)

**6.2.1.1.4 Support Vector Machines** <span id="6.2.1.1.4"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 7: Machine Learning III”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: "[Chapter 7: Machine Learning
    III](https://resources.saylor.org/archived/wp-content/uploads/2011/11/CS405-6.2.1.1.3-MIT.pdf)”
    (PDF)  
        
     Instructions: Read slide 7.4.24, in 6.034 Notes: Section 7.4, on
    the relationship of neural nets and SVMs (support vector
    machines).   
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF)

-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 8: Machine Learning IV”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: "[Chapter 8: Machine Learning
    IV](https://resources.saylor.org/archived/wp-content/uploads/2011/11/CS405-6.1.3.2-MIT-PartII.pdf)”
    (PDF)  
        
     Instructions: Read the slides in 6.034 Notes: Sections 8.1, 8.2,
    and 8.3.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF)

**6.2.1.2 "No Free Lunch" Theorem** <span id="6.2.1.2"></span> 
*Note: The reading of 6.2.1.1.4, slides 8.3.28 and 8.3.29, is applicable
to this section.  They give an indication of the challenges and
successes of supervised learning.*

-   **Reading: Wikipedia: “Supervised Learning”**
    Link: Wikipedia: ["Supervised
    Learning"](https://resources.saylor.org/archived/wp-content/uploads/2011/11/CS405-6.2.1.2-WIKIPEDIA.pdf)
    (PDF)  
        
     Instructions: Select the link and read the beginning of “Supervised
    learning.”  There are many learning methods, each having strengths
    and weaknesses in particular applications, for particular data sets
    and situations.  Issues that have to be contended with include: bias
    (a predicted value of a learning algorithm is systematically
    incorrect when trained on several different data sets) and variance
    (variation of a predicted value for a given input when trained on
    different data sets), complexity of functions to be predicted,
    complexity of data, noisy data, missing data, etc.  
        
     The “No Free Lunch Theorem” states, informally, that no one method
    works best for all applications and situations.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-Share-Alike License
    3.0](http://creativecommons.org/licenses/by-sa/3.0/) (HTML).  You
    can find the original Wikipedia version of this article
    [here](http://en.wikipedia.org/wiki/Supervised_learning) (HTML).

**6.2.2 Unsupervised** <span id="6.2.2"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 4: Learning Introduction”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course: ["Chapter 4: Learning
    Introduction"](https://resources.saylor.org/archived/wp-content/uploads/2011/11/CS405-6.1-MIT.pdf)
    (PDF)  
        
     Instructions: Read slide 4.1.9 on Clustering.   
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/) (PDF).

-   **Reading: UCI: Max Welling’s ICS 171 Introduction to Artificial
    Intelligence Course: Slides Lecture 9 (Learning)**
    Link: UCI: Max Welling’s ICS 171 Introduction to Artificial
    Intelligence Course: “[Slides Lecture 9
    (Learning)](http://www.ics.uci.edu/~welling/teaching/ICS171spring07/ICS171spring07.html)”
    (PPT)  
        
     Instructions: Select the PowerPoint file slides lecture 9
    (Learning) and read slides 3 and 4.  
        
     Terms of Use: Please respect the copyright and terms of use
    displayed on the webpages above.

**6.2.2.1 Difference From Supervised Learning** <span
id="6.2.2.1"></span> 
*Note: In unsupervised learning the data is not labeled and function
value pairs are not provided, as in supervised learning.  Approaches to
unsupervised learning try to discover patterns in the data. Some of the
material on supervised learning applies to unsupervised learning.*

**6.2.2.2 Unsupervised Methods** <span id="6.2.2.2"></span> 
*Note: Approaches used for unsupervised learning include clustering,
feature extraction, and neural nets. *

-   **Reading: Wikipedia: “Unsupervised Learning”**
    Link: Wikipedia: ["Unsupervised
    Learning"](https://resources.saylor.org/archived/wp-content/uploads/2011/11/CS405-6.2.2.2-WIKIPEDIA.pdf)
    (PDF)  
        
     Instructions: Select the link and read the beginning of
    “Unsupervised learning.”  There are many learning methods, each
    having strengths and weaknesses in particular applications, for
    particular data sets and situations.  Some issues that have to be
    contended with include: complexity of functions to be predicted,
    complexity of data, noisy data, missing data, etc.  
        
     As for supervised learning, see 6.2.1.2 above.  The “No Free Lunch
    Theorem” applies to unsupervised learning.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-Share-Alike License
    3.0](http://creativecommons.org/licenses/by-sa/3.0/) (HTML).  You
    can find the original Wikipedia version of this article
    [here](http://en.wikipedia.org/wiki/Unsupervised_learning) (HTML).

**6.2.2.2.1 Clustering** <span id="6.2.2.2.1"></span> 
-   **Reading: MIT: Kaelbling and Lozano-Perez 6.034 Artificial
    Intelligence Course: “Chapter 8: Machine Learning IV”**
    Link: MIT: Kaelbling and Lozano-Perez 6.034 Artificial Intelligence
    Course:["Chapter 8: Machine Learning
    IV"](https://resources.saylor.org/archived/wp-content/uploads/2011/11/CS405-6.1.3.2-MIT-PartII.pdf)
    (PDF)  
        
     Instructions: Read the indicated slides in 6.034 Notes: Sections
    8.4: see slides 8.4.18–8.4.21 and slides 8.4.47–8.4.64.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-ShareAlike License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Leslie Kaelbling and Tomás Lozano-Pérez and the
    original version can be found
    [here](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-spring-2005/lecture-notes/)
    (PDF).

-   **Lecture: Stanford University: Ng CS229 Machine Learning Course:
    “Lecture 12”**
    Link: Stanford University: Ng CS229 Machine Learning Course:
    “[Lecture
    12](http://see.stanford.edu/see/lecturelist.aspx?coll=348ca38a-3a6d-4052-937d-cb017338d7b1)”
    (Silverlight, YouTube, iTunes, WMV, or MP4)  
        
     Instructions: Select the link and then scroll down to Lecture 12.
    Choose your preferred format and watch the video lecture by
    Professor Ng on unsupervised learning.  
        
     Terms of Use: Please respect the copyright and terms of use
    displayed on the webpages above.

**6.2.2.2.2 K-Means** <span id="6.2.2.2.2"></span> 
*Note: The reading and video of 6.2.2.2.1 apply to this subunit.  From
the reading, see slides 8.4.22–8.4.36*

**6.2.2.2.3 Gaussian Mixture Models** <span id="6.2.2.2.3"></span> 
-   **Lecture: Stanford University: Ng CS229 Machine Learning Course:
    “Lecture 13”**
    Link: Stanford University: Ng CS229 Machine Learning Course:
    “[Lecture
    13](http://see.stanford.edu/see/lecturelist.aspx?coll=348ca38a-3a6d-4052-937d-cb017338d7b1)”
    (Silverlight, YouTube, iTunes, WMV, or MP4)  
        
     Instructions: Select the link and scroll down to Lecture 13. 
    Choose your preferred format and watch the video lecture by
    Professor Ng on additional approaches to unsupervised learning.  
        
     Terms of Use: Please respect the copyright and terms of use
    displayed on the webpages above.

**6.2.2.2.4 Principal Component Analysis** <span id="6.2.2.2.4"></span> 
-   **Lecture: Stanford University: Ng CS229 Machine Learning Course:
    “Lecture 14”**
    Link: Stanford University: Ng CS229 Machine Learning Course:
    “[Lecture
    14](http://see.stanford.edu/see/lecturelist.aspx?coll=348ca38a-3a6d-4052-937d-cb017338d7b1)”
    (Silverlight, YouTube, iTunes, WMV, or MP4)  
        
     Instructions: Select the link and scroll down to Lecture 14. Choose
    your preferred format and watch the video lecture by Professor Ng on
    Principal Component Analysis (PCA) for unsupervised learning.  
        
     Terms of Use: Please respect the copyright and terms of use
    displayed on the webpages above.

-   **Lecture: Stanford University: Ng CS229 Machine Learning Course:
    “Lecture 15”**
    Link: Stanford University: Ng CS229 Machine Learning Course:
    “[Lecture
    15](http://see.stanford.edu/see/lecturelist.aspx?coll=348ca38a-3a6d-4052-937d-cb017338d7b1)”
    (Silverlight, YouTube, iTunes, WMV, or MP4)  
        
     Instructions: Select the link and scroll down to Lecture 15.  Watch
    the video lecture by Professor Ng, which continues the presentation
    on Principal Component Analysis (PCA) and then goes on to introduce
    Independent Component Analysis (ICA).  
        
     Terms of Use: Please respect the copyright and terms of use
    displayed on the webpages above.

**6.2.2.2.5 Neural Network Models: SOM and ART** <span
id="6.2.2.2.5"></span> 
**6.2.2.2.5.1 SOM** <span id="6.2.2.2.5.1"></span> 
-   **Reading: Wikipedia: “Self-Organizing Map”**
    Link: Wikipedia: “[Self-Organizaing
    Map](https://resources.saylor.org/archived/wp-content/uploads/2011/11/CS405-6.2.2.2.5.1-WIKIPEDIA.pdf)”
    (PDF)  
        
     Instructions: Self-organizing Map (SOM) is a neural net model
    applied to unsupervised learning.  Look over the summary of this
    model in this reading.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-Share-Alike License
    3.0](http://creativecommons.org/licenses/by-sa/3.0/) (HTML).  You
    can find the original Wikipedia version of this article
    [here](http://en.wikipedia.org/wiki/Self-organizing_map) (HTML).

**6.2.2.2.5.2 ART** <span id="6.2.2.2.5.2"></span> 
-   **Reading: Wikipedia: “Adaptive Resonance Theory”**
    Link: Wikipedia: “[Adaptive Resonance
    Theory](https://resources.saylor.org/archived/wp-content/uploads/2011/11/CS405-6.2.2.2.5.2-WIKIPEDIA.pdf)”
    (PDF)  
        
     Instructions: Adaptive resonance theory (ART) is another neural net
    model applied to unsupervised (and also supervised) learning.  Look
    over the summary of this model in this reading.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-Share-Alike License
    3.0](http://creativecommons.org/licenses/by-sa/3.0/) (HTML).  You
    can find the original Wikipedia version of this article
    [here](http://en.wikipedia.org/wiki/Adaptive_resonance_theory)
    (HTML).

**6.2.2.2.6 Some Issues with Unsupervised Learning** <span
id="6.2.2.2.6"></span> 
*Note: the reading of 6.2.2.2.1 applies to this subunit.  See slides
8.4.48–8.4.64.*

**6.2.3 Semi-Supervised** <span id="6.2.3"></span> 
**6.2.3.1 Difference from Supervised Learning** <span
id="6.2.3.1"></span> 
-   **Reading: Wikipedia: “Semi-Supervised Learning”**
    Link: Wikipedia: ["Semi-Supervised
    Learning"](https://resources.saylor.org/archived/wp-content/uploads/2011/11/CS405-6.2.3.1-WIKIPEDIA.pdf)
    (PDF)  
        
     Instructions: Select the link and read the summary of
    semi-supervised learning.  
        
     Note: Semi-supervised learning involves labeled and unlabeled
    data.  It is a practical approach, in that it is comparatively
    inexpensive to obtain a large amount of unlabeled data and a small
    amount of labeled data, which together result in improved learning
    accuracy (over unsupervised learning).  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-Share-Alike License
    3.0](http://creativecommons.org/licenses/by-sa/3.0/) (HTML).  You
    can find the original Wikipedia version of this article
    [here](http://en.wikipedia.org/wiki/Semi-supervised_learning)
    (HTML).  

**6.2.3.2 Semi-supervised Methods** <span id="6.2.3.2"></span> 
*Note: Semi-supervised methods include co-training and joint
probability.*

**6.2.3.2.1 Co-Training** <span id="6.2.3.2.1"></span> 
-   **Reading: Wikipedia: “Co-Training”**
    Link: Wikipedia:
    "[Co-Training](https://resources.saylor.org/archived/wp-content/uploads/2011/11/CS405-6.2.3.2.1-WIKIPEDIA.pdf)”
    (PDF)  
        
     Instructions: Select the link and read the summary of this
    semi-supervised learning method.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-Share-Alike License
    3.0](http://creativecommons.org/licenses/by-sa/3.0/) (HTML).  You
    can find the original Wikipedia version of this article
    [here](http://en.wikipedia.org/wiki/Co-training) (HTML).

**6.2.3.2.2 Joint Probability** <span id="6.2.3.2.2"></span> 
-   **Reading: Stanford University: Ieong CS229 Machine Learning Course:
    “Handouts Probability Theory Review”**
    Link: Stanford University: Ieong CS229 Machine Learning Course:
    “[Probability Theory
    Review](https://resources.saylor.org/archived/wp-content/uploads/2011/11/CS405-6.2.3.2.2-STANFORD.pdf)”
    (PDF)  
        
     Instructions: Select the link and read section 1.3, which describes
    joint distributions.  Joint distributions from Probability Theory
    are useful for studying semi-supervised learning.  Two statistical
    techniques that are also helpful are maximum likelihood and
    expectation maximization, both of which are used to estimate the
    parameters of statistical models.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution License
    3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) (HTML).  It
    is attributed to Stanford University and the original version can be
    found
    [here](http://see.stanford.edu/see/materials/aimlcs229/handouts.aspx)
    (PDF).

**6.2.3.2.2.1 Maximum Likelihood** <span id="6.2.3.2.2.1"></span> 
-   **Reading: Wikipedia: “Maximum Likelihood”**
    Link: Wikipedia: “[Maximum
    Likelihood](https://resources.saylor.org/archived/wp-content/uploads/2011/11/CS405-6.2.3.2.2.1-WIKIPEDIA.pdf)”
    (PDF)  
        
     Instructions: Select the link and read the summary of maximum
    likelihood, a statistical method for estimating the parameters of a
    model.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-Share-Alike License
    3.0](http://creativecommons.org/licenses/by-sa/3.0/) (HTML).  You
    can find the original Wikipedia version of this article
    [here](http://en.wikipedia.org/wiki/Maximum_likelihood) (HTML).  

**6.2.3.2.2.2 Expectation Maximization** <span id="6.2.3.2.2.2"></span> 
-   **Reading: Wikipedia: “Expectation maximization”**
    Link: Wikipedia: “[Expectation
    maximization](https://resources.saylor.org/archived/wp-content/uploads/2011/11/CS405-6.2.3.2.2.2-WIKIPEDIA.pdf)”
    (PDF)  
        
     Instructions: Select the link and read the summary of expectation
    maximization, another statistical method for estimating the
    parameters of a statistical model.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-Share-Alike License
    3.0](http://creativecommons.org/licenses/by-sa/3.0/) (HTML).  You
    can find the original Wikipedia version of this article
    [here](http://en.wikipedia.org/wiki/Expectation_maximization)
    (HTML).  

**6.3 A Practical Tool for Machine Learning** <span id="6.3"></span> 
-   **Reading: Mark Watson’s Practical Artificial Intelligence
    Programming with Java: “Chapter 8: Machine Learning with Weka”**
    Link: Mark Watson’s *Practical Artificial Intelligence Programming
    with Java*: “[Chapter 8: Machine Learning with
    Weka](https://resources.saylor.org/archived/wp-content/uploads/2011/11/CS405-1.1-WATSON.pdf)”
    (PDF)  
        
     Instructions: Select the above link and read chapter 8, pages
    129–136, which briefly describe tool support for machine learning.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-NonCommercial-NoDerivs Unported License
    3.0](http://creativecommons.org/licenses/by-nc-nd/3.0/) (HTML).  It
    is attributed to Mark Watson and the original version can be found
    [here](http://markwatson.com/opencontent/JavaAI3rd.pdf) (PDF). 


