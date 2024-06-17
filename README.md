# Optimering eksamen på AU - Potentielle emner til dispositioner (Optimization Exam - Potential Topics)
Potential topics for the oral exam in the Optimization (dOpt / Opt) course at Aarhus Universitet / Aarhus University (AU). Good luck!
Disclaimer: Not made by me.

* [Kursuskatalog](https://kursuskatalog.au.dk/da/course/117969/Optimering)
* [Course Catalogue](https://kursuskatalog.au.dk/en/course/117969/Optimization)

## Note
The following is just a personal suggestion; you do not have to stick to this. If you find some other topic more interesting and easier to explain, you should do it. This is just to help you get started with the preparation.

## Topic 1: LP model and LP algorithms
In this, the highlight is the Simplex algorithm. You can start by defining the standard LP quickly and then you have two options: you can focus on the algorithm or you can focus on the theory.

If you focus on the algorithm, you can explain the two-phase simplex algorithm. You can talk about one-phase simplex, two-phase simplex, etc. The core of the algorithm is the pivoting rule, and this should be explained clearly. You can also mention why the algorithm terminates and why it outputs a correct solution. If you have time, you can mention the time complexity.

If you focus on the theory, you can explain the simplex algorithm (mainly the pivoting method) and then go on to talk about basic feasible solutions. One of the results due to which simplex works is the following: an optimal solution is a basic feasible solution (you have also seen an extension of this result in handin-4). Giving at least a proof by picture for this theorem is good. I think that even if you do not prove this, at least stating it is a good idea.

In the end, you can mention faster algorithms such as the Ellipsoid method or the Interior Point method. Here you should not spend too much time on how to convert any LP to a standard LP. Rather you should start with a standard LP and focus on the algorithm.

## Topic 2: LP Duality, Matrix Games, and ILP
Here, you have three options as evident from the title.

### First option: LP Duality
You should start with the definition of a dual LP (you can spend a minute or something explaining what is the purpose of a dual and why we arrive at the dual LP). After this, you can decide to go for some theoretical results like strong duality and complementary slackness. In strong duality, state the result clearly and then also mention the immediate corollaries (if primal is unbounded, then dual is infeasible, and so on). For complementary slackness, be careful in stating it, because there is a close relative, strict complementary slackness.  You can try to present the proof of complementary slackness as it is short (you can skip the algebra). If you are comfortable with the proof of strong duality, then you can present the intuition and high level idea of the proof. If you prefer not to present the proof, then it would be a good idea to talk briefly about an application of strong duality, such as min-max theorem.

### Second option: Matrix Games
Here you can start by defining the setup of matrix games (give the definition in an abstract way, i.e. Alice is maximiser, Bob is minimiser, they have a pay-off matrix, and so on). Then you can mention different types of games, such as symmetric games, zero-sum games, etc. For us, zero sum games are interesting. Then you can define equilibrium and conclude by talking about the existence of Nash Equilibrium in zero-sum games (min-max theorem). You can try to present the proof of this.

### Third option: ILP
Here you can start by stating the additional constraint of integers, and also say how having Boolean valued variables allow us to model several interesting problems as LP. Then you can describe ILPs of some problems such as Set cover and then shift your focus to TSP. While describing the ILP for TSP, explain clearly how you arrived at the constraints. You can also mention that ILP is NP-hard, and if time is still there, talk about branch and bound.

## Topic 3: Network Flow Models and Flow Algorithms
Here, you have two options.

### First option: Network Flow Models
In this, you can start by quickly describing the network flow problem, with the arc and node constraints, sink and source constraint, etc. After that, you can talk about the Totally Unimodular system and state the very cool result - all basic solutions of TUM are integral. Using this you can mention the integrality theorem for flows with integral constraints and capacities. In the end, you can spend two-three minutes on the celebrated theorem - max-flow min-cut theorem. If you are comfortable with the proof of max-flow min-cut, then you can present a high level idea of the proof with enough details.

### Second option: Flow Algorithms
In this, there are two algorithms - Ford-Fulkerson and Edmonds-Karp. Edmonds-Karp is a clever version of Ford-Fulkerson. So you can focus on the Edmond-Karps algorithm mostly, with clearly explaining the residual flow and the algorithm. Edmonds-Karp is better than Ford-Fulkerson in time complexity. So you should mention both the time complexity and then compare them. The difference arises in how the two algorithms try to increment the cost of the flow - Ford-Fulkerson does by incrementing the flow value (thus the running time depends on the value of the flow), on the other hand Edmonds-Karp does it by saturating the edges (thus the running time is polynomial in the input graph).

## Topic 4: P, NP, and Cook's Theorem
In this topic, the highlight is the famous Cook's Theorem. You can start by quickly defining the class P and NP. Then you can describe polynomial time reductions and then mention NP-hardness. After that, you can describe the SAT and Circuit-SAT problem, and next state the Cook's Theorem. The proof of Cook's Theorem consists of two steps - first step is to reduce Circuit-SAT to SAT, and the second step is to show that Circuit-SAT is NP-hard. You should try to do the first part, that is the easier part. If you are comfortable with the proof for the second step, then you should go for it, because it is quite important. In the end, if you have time, then you can talk about coNP, coNP complete problems, etc (refer to Tutorial 10).

## Topic 5: NP-Complete Problems
This topic is all about reductions showing that certain problems are NP-complete. In this, you can aim to cover 1 or 2 interesting and important reductions, such as MAX-2-SAT, MAXIMUM INDEPENDENT SET, 3-COLOR, MAX-CUT, and KNAPSACK. While presenting the reduction, focus on the gadgets, how they are used but do not spend too much time in the tiny details. Also show why the YES instances are mapped to YES instances and NO instances are mapped to NO instances, and why the reduction is running in polynomial time. You can conclude your presentation by talking about pseudo-polynomial time algorithms and strong NP-completeness. You have seen (two) pseudo-polynomial time algorithms for KNAPSACK but KNAPSACK is NP-complete (but not strongly NP-complete). You can refer to Papadimitrou Section 9.4 for more thorough discussion. If you have some time, you can also talk about the consequences if a NP-complete problem is in coNP (refer to Tutorial 10).

## Topic 6: Approximation Algorithms
Here you have two options.

### First option:
You can talk about different kinds of approximation algorithms such as randomized, relaxation of LP and rounding, and greedy. For randomized, you can use MAX-3-SAT or MAX-CUT (both are pretty similar, so use any one of them). You can present the analysis of the randomized algorithm because it is simple and clean (note that the magic happens because of linearity of expectation, or else we cannot say much about the sum of random variables). For rounding, you can use the Minimum weighted vertex cover as presented in the lecture. For greedy, you can use Knapsack or MAX-CUT. You can aim to cover two of these three techniques.

### Second option:
Here you can focus on approximation algorithms for TSP (refer to Lecture 26 and 27).

## General remarks:
1. State the theorems precisely, like what is the exact hypothesis, exact result, etc. Similarly clearly describe the algorithms or reductions. This will ensure that you have understood and gained the important results from this course.
2. Do try to prove at least one interesting result or a reduction completely, i.e. something concrete. This will ensure you have a firm grip in the technical part of the course.
3. Do not spend too much time in tiny details, rather focus on the big picture, intuition, ideas. This will ensure you can recognise the key concepts and ideas.
4. Do not assume that the examiners will be familiar with your notation or anything. So anything you are going to write on the whiteboard, state what it is.
5. Try to make a presentation for 8-9 minutes, leaving some room for yourself and the examiners to ask you something.
