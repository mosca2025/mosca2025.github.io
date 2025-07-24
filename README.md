22 July 2025 (Tuesday)\
[CAV 2025](https://conferences.i-cav.org/2025/)\
[University of Zagreb, Faculty of Electrical Engineering and Computing](https://www.google.com/maps/place/Faculty+of+Electrical+Engineering+and+Computing/@45.8003692,15.968797,17z/data=!3m1!4b1!4m6!3m5!1s0x4765d6f150cf2ccd:0x739e5c279fd98531!8m2!3d45.8003692!4d15.9713773!16zL20vMGd3dDd3?entry=ttu&g_ep=EgoyMDI1MDMxNy4wIKXMDSoJLDEwMjExNDUzSAFQAw%3D%3D)\
Zagreb, Croatia

## Description

String is a basic data type in almost every programming language and has been widely used in many scenarios, especially web programming. String constraint solving is a classical topic in theoretical computer science. A seminal result is the decidability of the theory of word equations shown by Makanin in 1977. String constraint solving has received much more attention in the last decade, as a result of the momentum from formal verification of string-manipulating programs. Various string constraint solvers have been developed, e.g. Z3-str3, cvc5, Norn, Trau, Ostrich, and Z3-Noodler. Furthermore, various verification and testing tools, e.g. jDART for Java, Jalangi for Javascript, and PyExZ3 for Python, have been developed based on string constraint solvers.

Nevertheless, string constraint solving and formal verification of string-manipulating programs, compared to the counterpart for integer data type, are still rather immature. Firstly, state-of-the-art string constraint solvers still face serious precision and scalability issues. Furthermore, formal verification techniques and tools for string manipulating programs are still in their infancy, e.g. there are only a few works on deductive verification and model checking of string-manipulating programs.

The primary aim of the workshop is to provide a forum for researchers with interests in string constraint solving and formal verification of string-manipulating programs to exchange ideas and techniques, aiming at fostering fruitful research related to strings in the following years.

This workshop can be seen as a follow-up workshop of [MOSCA 2019](https://mosca19.github.io/) and [MOSCA 2023](https://mosca2023.github.io/).

## Organizers

* [Joel Day](https://www.lboro.ac.uk/departments/compsci/staff/joel-day/), Loughborough University, UK
* [Matthew Hague](https://www.cs.rhul.ac.uk/home/uxac009/), Royal Holloway University of London, UK
* [Ondřej Lengál](https://www.fit.vut.cz/person/lengal/), Brno University of Technology, Czech Republic

## Confirmed Speakers (alphabetical)

* Rachel Cleaveland (Stanford University)
* Dominik D. Freydenberger (Loughborough University)
* Vojtěch Havlena (Brno University of Technology)
* Michal Hečko (Brno University of Technology)
* John Zhengyang Lu (University of Waterloo)
* Oliver Markgraf (RPTU Kaiserslautern)
* Margus Veanes (Microsoft)
* Georg Zetzsche (MPI-SWS)

## Programme

| Time                 | Programme   |
|:--------------------:|-----------|
| 9:00   | [Slice closures of indexed languages and word equations with counting constraints](https://github.com/mosca2025/mosca2025.github.io/raw/master/slides/mosca25-georg-zetzsche.pdf) (Georg Zetzsche) |
| 9:45   | [Finite Models for the Theory of Concatenation](https://github.com/mosca2025/mosca2025.github.io/raw/master/slides/mosca25-dominik-freydenberger.pdf) (Dominik D. Freydenberger)      |
| <span style="color:green">10:30</span>  |  <span style="color:green">☕️Coffee break☕️</span> |
| 11:00 | [Solving String Constraints via Regular Constraint Propagation](https://github.com/mosca2025/mosca2025.github.io/raw/master/slides/mosca25-oliver-markgraf.pdf) (Oliver Markgraf) |
| 11:30 | [Monte Carlo Tree Search for SMT Strategy Synthesis with Applications to String Constraints](https://github.com/mosca2025/mosca2025.github.io/raw/master/slides/mosca25-john-lu.pptx) (John Zhengyang Lu) |
| <span style="color:green">12:00</span> | <span style="color:green">🥗Lunch🥗</span> |
| 14:00 | [Handling Position Constraints Uniformly Including the Negated Containment](https://github.com/mosca2025/mosca2025.github.io/raw/master/slides/mosca25-michal-hecko.pdf) (Michal Hečko) |
| 14:45 | Theory and Applications of Symbolic Derivatives for ERE (Margus Veanes) |
| <span style="color:green">15:30</span> | <span style="color:green">☕️Coffee break☕️</span> |
| 16:00 | [Incorporating Native String Reasoning in Symbolic Execution of C Programs](https://github.com/mosca2025/mosca2025.github.io/raw/master/slides/mosca25-rachel-cleaveland.pdf) (Rachel Cleaveland) |
| 16:30 | [Z3-Noodler 1.3: Shepherding Decision Procedures](https://github.com/mosca2025/mosca2025.github.io/raw/master/slides/mosca25-vojtech-havlena.pdf) (Vojtěch Havlena) |
| 17:00 | <span style="color:red">reserve<span> |
| 17:30 | end of programme |


## Venue

University of Zagreb, Faculty of Electrical Engineering and Computing\
Unska ul. 3\
Zagreb, Croatia

<iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d5563.0873365271955!2d15.971377299999999!3d45.8003692!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x4765d6f150cf2ccd%3A0x739e5c279fd98531!2sFaculty%20of%20Electrical%20Engineering%20and%20Computing!5e0!3m2!1sen!2sus!4v1743628327445!5m2!1sen!2sus" width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>

## Talk Abstracts

### Rachel Cleaveland (Stanford University) --- Incorporating Native String Reasoning in Symbolic Execution of C Programs
Symbolic execution is a powerful program analysis technique that explores new paths through a program by generating inputs that are guaranteed to exercise these paths. However, there is a lack of modern research on symbolic execution for programs that manipulate string data. Existing engines for string-manipulating programs suffer from two major drawbacks. First, these existing tools only execute Java programs, leaving the topic of symbolic execution for string-manipulating programs in languages like C unstudied. Second, most of these tools implement bespoke string solvers that are not under active development, and therefore do not integrate the vast improvements to string solvers that we have seen in the past decade.
Due to these drawbacks in prior work, we develop a tool called SymCC-STR to symbolically execute C programs that operate on strings. SymCC-STR is built on top of the concolic execution engine SymCC and uses the smt-switch SMT solving API in the backend, so it makes use of modern advancements in both symbolic execution and string solving.
SymCC-STR implements a novel hybrid data representation, expressing symbolic data both as SMT bitvectors and as SMT strings in order to balance the performance and expressivity of these respective theories. While SymCC-STR is still under active development, preliminary results from symbolically executing real-world programs indicate that SymCC-STR is able to cover branches that previous methods miss.

### Dominik D. Freydenberger (Loughborough University) --- Finite Models for the Theory of Concatenation
Word equations are one of the most natural and intuitive models in theoretical computer science. A (still quite) natural next step is combining word equations with first-order logic. The resulting theory of concatenation is elegant; sadly, its satisfiability problem is undecidable. 

If we assume that the universe is not the set of all strings over a given alphabet, but instead one string and all its factors, we get a meaningful distinction between satisfiability and model checking. While the former remains undecidable, the latter is not only decidable, but can be made tractable by building on techniques from finite model theory.

This talk aims to give a short introduction to this approach, including applications to regular expressions with back-references.

### Vojtěch Havlena (Brno University of Technology) --- Z3-Noodler 1.3: Shepherding Decision Procedures
Z3-Noodler is a fork of the Z3 SMT solver replacing its string theory implementation with a portfolio of decision procedures and a selection mechanism for choosing among them based on the features of the input formula. In this talk, I will give an overview of the used decision procedures, important heuristics, and their integration into a robust solver with a good overall performance, as witnessed by Z3-Noodler winning the string division of SMT-COMP'24.

### Michal Hečko (Brno University of Technology) --- Handling Position Constraints Uniformly Including the Negated Containment
I will present a novel approach to solving the so-called position predicates in combination with regular constraints restricting the language of variables. Position predicates, e.g., string disequation, NotPrefix, NotSuffix, etc., are a large set of practically-relevant string constraints whose satisfiability witness is an interesting position(s) within strings assigned to variables. Our approach provides a uniform framework for these predicates that tightly integrates their semantics with a symbolic description of runs of automata associated with the string variables, resulting in a reduction to quantifier-free linear integer arithmetic. I will give a gradual exposition of the key ideas powering the reduction, allowing us to avoid exponential blow-up and to show that the entire examined fragment of string logic is NP-complete. In the case of only a single position constraint, we give a decision procedure that works in PTime. We implemented the approach in the string solver Z3-Noodler, showing the practicality of our approach in the presence of word equations that allow monadic decomposition, i.e., the chain-free fragment.
In the second part of my talk, I will focus on the negated string containment predicate and provide a positive answer to its decidability, which was, for a long time, an open problem. The semantics of the negated string containment include universal quantification, making the problem intractable by reducing it to word equations and placing it on the boundary of decidability. The exposition of our proof starts with why and when our uniform approach to position constraints can provide a decision procedure. I will then provide a high-level intuition behind two key theorems based on combinatorics on words that power our result, while aiming at keeping the exposition informal and approachable. Finally, I will discuss future directions of our work.

### John Zhengyang Lu (University of Waterloo) --- Monte Carlo Tree Search for SMT Strategy Synthesis with Applications to String Constraints
Z3 allows users to customize strategies to improve performance on their specific use cases. However, manually designing an optimized strategy for a given class of SMT instances remains a complex and demanding task. Recently, we proposed Z3alpha, a method based on Monte Carlo Tree Search (MCTS) to automate SMT strategy synthesis. Z3alpha has demonstrated strong performance on some challenging logics such as QF_NIA and QF_NRA. In this talk, we will present the core ideas behind Z3alpha and highlight its application to string constraints. We will also discuss the insights it provides, such as identifying which strategies work best for different families of string problems.

### Oliver Markgraf (RPTU Kaiserslautern) --- Solving String Constraints via Regular Constraint Propagation
String constraints appear widely in program analysis and security applications, yet solving them efficiently remains a challenge due to the complexity of string operations. In this talk, I will present Regular Constraint Propagation (RCP), a lightweight and generic approach for solving such constraints. RCP infers information by computing pre- and post-images of regular languages under string functions like concatenation and replace, enabling propagation through complex constraints. I will outline the key ideas behind RCP, demonstrate its theoretical guarantees, and show how it is implemented in the OSTRICH solver. Experimental results highlight that RCP not only broadens the solver’s applicability but also improves performance—especially on random PCP and bioinformatics benchmarks. The talk will focus on the intuition, algorithmic structure, and practical impact of RCP. This is joint work with Matthew Hague, Artur Jeż, Anthony Widjaja Lin and Philipp Rümmer.

### Margus Veanes (Microsoft) --- Theory and Applications of Symbolic Derivatives for ERE
The aim of this talk is to explain the theory and the algorithmic principles behind the theory of
symbolic derivatives of extended regular expressions (ERE) and how they can benefit matching and constraint solving.
The focus will be on how the theory efficiently supports,  in addition to the classical operators,
also complement, intersection and a restricted form of regex lookarounds.
In the latter case using span semantics that generalizes language semantics. As concrete examples of
applications of the theory, I will talk about: ERE matching, Guidance of LLM tokenization, and ERE constraint solving in SMT.
If time permits, I will also cover some aspects of using the theory for omega-regularity,
where derivatives are taken relative to stream (infinite word) semantics.

### Georg Zetzsche (MPI-SWS) --- Slice closures of indexed languages and word equations with counting constraints
Indexed languages are a classical notion in formal language theory. As the language equivalent of second-order pushdown automata, they have received considerable attention in higher-order model checking. Unfortunately, counting properties are notoriously difficult to decide for indexed languages: So far, all results about non-regular counting properties show undecidability.

In this paper, we initiate the study of slice closures of (Parikh images of) indexed languages. A slice is a set of vectors of natural numbers such that membership of u,u+v,u+w implies membership of u+v+w. Our main result is that given an indexed language L, one can compute a semilinear representation of the smallest slice containing L's Parikh image.

We present two applications. First, one can compute the set of all affine relations satisfied by the Parikh image of an indexed language. In particular, this answers affirmatively a question by Kobayashi: Is it decidable whether in a given indexed language, every word has the same number of a's as b's.

As a second application, we show decidability of (systems of) word equations with rational constraints and a class of counting constraints: These allow us to look for solutions where a counting function (defined by an automaton) is not zero. For example, one can decide whether a word equation with rational constraints has a solution where the number of occurrences of a differs between variables X and Y.

The talk is based on joint work with Laura Ciobanu and has appeared at LICS 2024.

