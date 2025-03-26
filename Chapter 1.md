# Chapter 1: Software Engineering Principles

## Software Design Process

Developing techniques and methodolgy to write software programs include:

*Problem Analysis*: Understanding the nature of the problem to be solved

*Requirements definition*: Specifying exactly what the program must do.

*High- and Low-level design*: Recording how the program meets the requirements.

*Implementation of the design*: Coding a program in a computer language.

*Testing and verification*: Detecting and fixing errors and demonstrating the correctness of the program.
*Delivery*: Turning over the tested progam to the customer or user (or instructor!)

*Operation* Actually using the program.

*Maintenece*: Making changes to fix operational errors and to add or modify functions of the program.

We can go though these steps one by one or concurrently, that should be kept in mind when designing new software.

We use the term *software engineering* to refer to a disciplied approach to the development of computer programs though all of these software life-cycle activities.

>**Software Engineering**: A disciplined approach to the design, production, and maintence of computer programs that are developed on time and within costs estimaes, using tools that help to manage the size and comlexity of the resulting software products.

>*Algorithm*: A logical sequence of discrete steps that describes a complete solution to a given problem computable in a finite amount of time.

## Goals of Quality Software

Quality software is muchr than a program that somehow accomplishes the task at hand. A good program achieves the following goals:

> It works.
>
> It can be read and understood.
>
> It can be modified without excruciating time and effort.
>
> It is completed on time and within budget.

***It's not easy to meet these goals, but they are important.***

*** Goal 1: Quality Software Works ***
The program must do the task it was designed to perform, and it must do it correctly and completely. To write a program that works you first need to have a definition of the program's *reqirements.*

> **Requirements:** A statement of what is to be provided by a computerd system or software product.

We develop programs that meet the user's requirements using *software specifications.* The specifications indicate the format of the input and the expected output.

> **Software Specification:** A detailed description of the function, inputs, processing, outputs, and special requirements of a software product. It provides the information needed to design and implement the program.

Goal 1 means that the program should be as *effcient as it needs to be.* We would never deliberately write programs that waste time or space in memory, but no all programs demand great efficiency.

### Goal 2: Quality Software Can Be Read and Understood

The second goal is more concered with our ability to read the program. reading a well-written program can teach you techniques that help you write good programs.

### Goal 3: Quality Software Can be Modified

When does software need to be modified? Changes occur in every phase of its existance.

> 1. Software gets changed in the testing phase.
> 2. Software gets changed in the coding phase.
> 3. Software gets changed in the testing phase.

The point is that software changes often and in all places of its life cycle. Knowing this, software engineers try to develop programs that are easily modifiable.
What makes a program easily modifiable? First, it should meet Goal 2: it should be readable and understandable to humans. Second, it should be able to witstand small changes easily. 

### Goal 4: Quality Software Is Completed on Time and Within Budget
Failure to meet deadlines is expensive.

## Specification: Understanding the Problem

> The first step is to *think*. Before you can come up with a program solution, you must understand the problem. Read the assignment, and then read it again. Ask questions of your instructor (or manager, or client). Start early affords you many opportunities to ask questions; starting the night beofre the program is due leaves you no oppportunity at all.

### Writing Detailed Specificiations
1. First write a complete defintion of the problem, including:
    - the details of the expected inputs and outputs,
    - the necessary processing and error handling,
    - all the assumptions about the problem.

The process of writing the specifications tells you exactly what the program should do.

*Detailed specification*: a formal defnition of th eproblem your program must solve.

## Program Design

The detailed specification fo the program tells what the progm must do, but not how it does it. Once you have fully claified the goals fo the program, you can begin to develop and record a strategy for meeting them; in other words, you can begin the design phase of the software life cycle.

### Abstraction

The universe is filled with comples systems. We use models to reduce the complexity with abstraction. An ***abstraction*** is a model of a comples system that includes only the essential details. Different abstractions of a particular system are used by different viewers of the system.

> **Abstraction**: A model of a complex system that includs only the details essential to the perspective of the viewer of the system.

## Information Hiding
One important feature of any design method is that the details that are specified in lower levels of the program design are hidden form the higher levels. The programmer sees only the details that are relevant at a particular level fo the design. This is *information hiding* makes certain details inaccessible to the programmer at higher levels.

> ***Infomration Hiding***: The practice of hiding the details ofa  function or data structure with the goal of controlling access to the details fo a module or structure.

Infomration hiding prevents the high levels of the design from becoming dependent on low-level design dedtails that are more likely to be changed. The concepts of abstraction and information hiding are fundamental principles of software engineering.

### Functional Decomposition
One method fo designing software is called ***functional decomposition***, also called ***top-down design***.
> First the problem is broken into several large tasks. Each of these tasks is in turn divided into sections, then the sections are subdivided, and so on. The important feature is that details are deferred as long as possible as we move from a general to a specific solution. ... The functional decomposition approach encourages programming in logical units, using functions. The main moduel of the design beomces the main program (also called the main function), and subsections develoop into funtions. The main module of the design becomes the main porogram, and the subsections develop into fuctions. This *hierachy of tasks* forms the basis for functional decomposition, with the main program or function controlling the processing.

> In functional decomposition, infomration hiding is accomplished primarly though dferring the details of algorithmns. This form of information hiding is based on *procedural* or *functional abstraction*.

### Object-Oriented Design

*Object-oriented design* originalted with the develoopment of programs to simulate physical objects and process in the real world.

In object-oriented design, the first step is to identify the simplest and most widely used objects and process in the decomposition and implement them faithfully. Once you have completed this stage, you often cna reuse these objects and process to implement more complex objects and process. This *hierachy of objects* is the basis for object-oriented design.

Groups of objects with similar properties and behaviors are described by ***object class*** (usually shorted to class).

> [!NOTE]
> ***Object Class (Class) The description of a group of objects with similar properties and behaviours; a pattern for creating individual objects.