# Expert_Systems

## History
Expert systems were introduced by the Stanford Heuristic Programming Project led by Edward Feigenbaum, who is sometimes termed the "father of expert systems";
other key early contributors were Bruce Buchanan and Randall Davis.

The Stanford researchers tried to identify domains where expertise was highly valued and complex, such as diagnosing infectious diseases (Mycin) and identifying unknown organic molecules (Dendral).

The idea that "intelligent systems derive their power from the knowledge they possess rather than from the specific formalisms and inference schemes they use" – as Feigenbaum said – was at the time
a significant step forward, since the past research had been focused on heuristic computational methods, culminating in attempts to develop very general-purpose problem solvers (foremostly the conjunct
work of Allen Newell and Herbert Simon).

Expert systems became some of the first truly successful forms of artificial intelligence (AI) software.

### 1 The project

The goal of this project is to make an expert system for propositional calculus.

### 2 What you have to do

You must implement a backward-chaining inference engine. Rules and facts will be given as a text file, the format of which is described in the appendix. A fact can be any uppercase alphabetical character. Your program must accept one parameter, which is the input file. It will contain a list of rules, then a list of initial facts, then a list of queries. For each of these queries, the program must, given the facts and rules given, tell if the query is true, false, or undetermined. By default, all facts are false, and can only be made true by the initial facts statement, or by application of a rule. A fact can only be undetermined if the ruleset is ambiguous, for example if I say "A is true, also if A then B or C", then B and C are undetermined. If there is an error in the input, for example a contradiction in the facts, or a syntax error, the program must inform the user of the problem. Here’s a list of the features we would like your engine to support. You can only get 100% of the grade by implementing all of them.

"AND" conditions. For example, "If A and B and [...] then X"
"OR" conditions. For example, "If C or D then Z"
"XOR" conditions. For example, "If A xor E then V". Remember that this means "exclusive OR". It is only true if one and only one of the operands is true.
Negation. For example, "If A and not B then Y"
Multiple rules can have the same fact as a conclusion
"AND" in conclusions. For example, "If A then B and C"
Parentheses in expressions. Interpreted in much the same way as an arithmetic expression.
