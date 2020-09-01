---
layout: post
title: Cyclomatic Complexity
---
Cyclomatic complexity is a software metric used to indicate the complexity of a program. It is a quantitative measure of the number of linearly independent paths through a program's source code.
Cyclomatic complexity is computed using the control flow graph of the program: the nodes of the graph correspond to indivisible groups of commands of a program, and a directed edge connects two nodes if the second command might be executed immediately after the first command. Cyclomatic complexity may also be applied to individual functions, modules, methods or classes within a program.
(https://en.wikipedia.org/wiki/Cyclomatic_complexity)
# V(G) = E(dges) - N(odes) + 2

CC  Code  Test  Maintain
1-10  Clear & well constructed  High  Low
10-20 Complex Middle  Middle
20-30 Very Complex  Low High
>30 Unreadable  Untestable  Very High

# Solutions
1. Factoring functions: put a block of codes into a function
2. Guard Clause: for some condition check, return immediately if no operation for the condition
3. Combine Conditions: combine condtions instead of multiple if checks
4. Polymorhpism Functions: use polymorphics functions to deal with complex conditions/inputs
5. Condition Function: use function that checks specific conditions
6. Simple Algorithm: use simpler algorithm
7. Reduce/remove Control Flags: Sometimes flags are used to signal a break of loops. Try to remove this kind of flags and use immediate return instead.
