---
layout: post
title: "Homework 2: Programming History"
#description: 
#headline:
#modified: year-month-day
#category: solution
#tags: []
#imagefeature: 
#mathjax: 
#chart: 
comments: true
featured: false
showSolution: false
---

{% comment %}

1.  What are the three common types of errors in computer programs? Provide an example for each category.  
    {% if site.showSolution==true and page.showSolution==true %}
    **Answer:**  
    1. syntax errors  
    2. runtime errors  
    3. semantic errors  
    See the lecture notes for examples of each category.
    {% endif %}

1.  Suppose you write a program that has memory leak. What type of programming error you dealing with?  
    {% if site.showSolution==true and page.showSolution==true %}
    **Answer:** runtime error
    {% endif %}

1.  Consider the following Bash script.  
    Identify the programmatic errors and their kinds (syntax, runtime, semantic) in this script.  
    Rewrite this script with the help of Linux cheatsheet in the lectures so that it does what the comments state.  
    ```Bash
    # make a new directory named `subdir` in the current directory.
    rm -rf ../subdir
    # change the directory to `subdir` directory in the current directory.
    mv ../subdir
    # create a new file named `newfile.md` in `subdir` directory.
    tuoch newfile.md
    # show the new file contents on the command line.
    tac newfile
    ```  
    {% if site.showSolution==true and page.showSolution==true %}
    **Answer:**  
    ```Bash
    # make a new directory named `subdir` in the current directory.
    mkdir ./subdir # two semantic errors. 
    # change the directory to `subdir` directory in the current directory.
    cd ./subdir # two semantic errors.
    # create a new file named `newfile.md` in `subdir` directory.
    touch newfile.md # one syntax error.
    # show the new file contents on the command line.
    cat newfile # one syntax error, one runtime error.
    ```  
    {% endif %}

{% endcomment %}

&#9827; **Due Date: Wednesday Oct 2, 2024 4:00 PM**.  
This homework aims at giving you some experience with computer hardware and software.  
Please write your answers in a `README.md` file and push them all to `hw/2/` folder of your repository on GitHub.  

1.  Consider [this programming history chart](./2/progLangChartPuzzle.pdf){:target="_blank"}, in which several programming language nodes are missing.  
    These languages are the following: lisp, basic, Algol 58, C, FORTRAN, Fortran 90, Python, C++, C#, Java, JavaScript, sh.  
    1.  Download the above PDF, add these languages to the right node in this fillable PDF file, save the file and submit it along with your answers to other questions.  
    1.  Sort the above languages chronologically and write them here.  
    1.  Write down the decade during which these languages were developed.  
    {% if site.showSolution==true and page.showSolution==true %}
    **Answer:**  
    See the lecture notes.  
    {% endif %}
    <br>

1.  What does ENIAC stand for?  
    {% if site.showSolution==true and page.showSolution==true %}
    **Answer:**  
    Electronic Numerical Integrator And Computer.  
    {% endif %}

1.  Why is everything represented by integers in computers?  
    {% if site.showSolution==true and page.showSolution==true %}
    **Answer:**  
    Because computers work with electricity current, and the electric current can be either on or off, representing 0 and 1.  
    {% endif %}

1.  What is the name of the fastest part of the computer memory?  
    {% if site.showSolution==true and page.showSolution==true %}
    **Answer:**  
    Register.  
    {% endif %}

1.  What is the slowest storage device in computers (that is typically integrated with computers)?  
    {% if site.showSolution==true and page.showSolution==true %}
    **Answer:**  
    Hard Drive.  
    {% endif %}

1.  What is the smallest unit of information in computer science?  
    {% if site.showSolution==true and page.showSolution==true %}
    **Answer:**  
    A bit, representing either 0 or 1.  
    {% endif %}

1.  (A) What is the closest programming language to machine code (i.e., binary code)?  
    {% if site.showSolution==true and page.showSolution==true %}
    **Answer:**  
    Assembly  
    {% endif %}
    (B) Does it need interpretation in order to become machine-comprehensible?  
    {% if site.showSolution==true and page.showSolution==true %}
    **Answer:**  
    Yes. An *Assembler* interprets the program for the machine.  
    {% endif %}

1.  (A) Name the oldest high-level programming language that is still in active daily use.  
    {% if site.showSolution==true and page.showSolution==true %}
    **Answer:**  
    Fortran  
    {% endif %}
    (B) Approximately how many decades is it old? ($\pm15$ years is acceptable answer. the decade it was created is also an acceptable answer)  
    {% if site.showSolution==true and page.showSolution==true %}
    **Answer:**  
    in 1950s  
    {% endif %}

1.  (A) Name a second-generation programming language.  
    {% if site.showSolution==true and page.showSolution==true %}
    **Answer:**  
    Assembly    
    {% endif %}
    (B) Which language-generation are Fortran, C, C++, MATLAB, Python, R?  
    {% if site.showSolution==true and page.showSolution==true %}
    **Answer:**  
    third, third, third, fourth, fourth, fourth  
    {% endif %}

1.  In what decades C, C++, and MATLAB/Python were created, respectively?  
    {% if site.showSolution==true and page.showSolution==true %}
    **Answer:**  
    1970s, 1980s, 1980s, 1990s  
    {% endif %}

1.  Name an ancestor programming language of C.  
    {% if site.showSolution==true and page.showSolution==true %}
    **Answer:**  
    B  
    {% endif %}

1.  Name a programming language ancestor of C++.  
    {% if site.showSolution==true and page.showSolution==true %}
    **Answer:**  
    C, Simula  
    {% endif %}

1.  Name a programming language ancestor of MATLAB and a programming language ancestor of Python.  
    {% if site.showSolution==true and page.showSolution==true %}
    **Answer:**  
    Fortran/C  
    {% endif %}

1.  What is fastest part of the memory in the memory hierarchy of modern computers?  
    {% if site.showSolution==true and page.showSolution==true %}
    **Answer:** register
    {% endif %}

1.  What is typically the smallest memory unit in the memory hierarchy of modern computers?  
    {% if site.showSolution==true and page.showSolution==true %}
    **Answer:** register
    {% endif %}

1.  How much faster is the access to the register memory compared to RAM in modern computers?  
    {% if site.showSolution==true and page.showSolution==true %}
    **Answer:** ~100 times.
    {% endif %}

1.  How much faster is the access to the RAM compared to typical SSD hard drives in modern computers?  
    {% if site.showSolution==true and page.showSolution==true %}
    **Answer:** ~1,000 times.
    {% endif %}

1.  How much faster is the access to the RAM compared to typical HDD hard drives in modern computers?  
    {% if site.showSolution==true and page.showSolution==true %}
    **Answer:** ~1,000,000 times.
    {% endif %}

1.  What are the primary roles of transistors in computers?  
    {% if site.showSolution==true and page.showSolution==true %}
    **Answer:** The form the basic logic gates and act as amplifiers.
    {% endif %}

1.  We know that more transistors mean faster computers.  
    Then, why cannot we add more transistors to computers to make them faster?  
    {% if site.showSolution==true and page.showSolution==true %}
    **Answer:** Transistors have become so small that making them smaller is nearly impossible.  
    {% endif %}

1.  What are the three tasks accomplished within a CPU cycle?  
    {% if site.showSolution==true and page.showSolution==true %}
    **Answer:** Fetch, decode, and execute instructions.  
    {% endif %}

1.  Can a powerful computer with more CPU cycles be slower than a computer with less CPU cycles? Why or How?  
    {% if site.showSolution==true and page.showSolution==true %}
    **Answer:** Yes, the computer speed depends on two primary factors: CPU cycles count and memory access speed.  
    {% endif %}

1.  What is the bottleneck of speed in modern computers? CPU clocks or memory access? Why?  
    {% if site.showSolution==true and page.showSolution==true %}
    **Answer:** CPUs are nowadays much faster than memory access.  
    Therefore memory access is the computer performance bottleneck.  
    {% endif %}

1.  What is the difference between the Dennard Scaling, MOSFET scaling, and Moore's law?  
    {% if site.showSolution==true and page.showSolution==true %}
    **Answer:** 
    Since the early days of invention of transistors, engineers realized that as the transistors get smaller, 
    their power consumption also reduces proportionally, such that the overall Power Density of transistors remains roughly the same. 
    This observation has become known as the **Dennard scaling**, also known as **MOSFET scaling** in honor of Robert H. Dennard 
    who was a co-author of a 1974 paper discussing this semi-empirical phenomenon.
    The Dennard Scaling implies that the more transistors we can fit on an Integrated Circuit (IC), 
    typically of size 1 centimeters, the faster the CPU will become. Short after the discovery of Dennard Scaling, 
    Gordon Moore, the former CEO of Intel, predicted in 1975 that the transistor count in microprocessors will double every two years. 
    His prediction held for multiple decades to become known as **Moore's law**.  
    {% endif %}

1.  Consider the following chessboard.  
    Suppose I ask you to put a single rice grain in the first square.  
    Then I ask you to put incrementally one more grain in each new square than the previous one:  
    1, 2, 3, 4, 5, ...
    1.  How many grains would you need to put in the last (64th) square?  
    1.  How many grains overall would you need to fill all chessboard squares incrementally as described above?  
    1.  A pound of rice is roughly 7000 grains. How many pounds of rice would you need for this task?  
    ![chessboard](./2/arithmetic.png)  
    {% if site.showSolution==true and page.showSolution==true %}
    **Answer:**  
    See the lecture notes.  
    {% endif %}
    <br>

1.  Consider the following chessboard.  
    Suppose I ask you to put a single rice grain in the first square.  
    Then I ask you to put in each subsequent square twice more than the previous square grains:  
    1, 2, 4, 8, 16, ...
    1.  How many grains would you need to put in the last (64th) square?  
    1.  How many grains would you need to fill the last chessboard square geometrically as described above?  
    1.  A pound of rice is roughly 7000 grains. How many pounds of rice would you need for this task?  
    1.  The current annual world production of rice is roughly $2\times10^{12} = 2,000,000,000,000$ lbs.  
        How many years will it take to produce the required amount of rice grains to place on this chessboard in this fashion?  
    ![chessboard](./2/geometric.jpg)  
    {% if site.showSolution==true and page.showSolution==true %}
    **Answer:**  
    See the lecture notes.  
    {% endif %}

1.  What are the three fundamental components of a Turing-complete language?  
    {% if site.showSolution==true and page.showSolution==true %}
    **Answer:**  
    1. a way for accessing the memory  
    2. a way for iteration  
    3. a way for branching  
    {% endif %}

1.  **Extra credit:** How would you distinguish exponential behavior vs. power-law behavior (function) in a 2-dimensional plot?  
    **Hint**: Recall our discussion of the ENAIC project and the relative frequency of keywords such as "computer" in our programming.  
    {% if site.showSolution==true and page.showSolution==true %}
    **Answer:**  
    An exponential curve looks like a line only when the X-axis is plotted on log-scale.  
    A power-law curve looks like a line only when both the X- and Y- axes are plotted on log-scale.  
    {% endif %}
