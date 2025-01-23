# Truth Table Generator
> #### Date created: December 2023
>
> ##### Written in: **Java**
>
> [Github](https://github.com/ElijahWood2003/truth-table-generator) 
<p>The goal of this project was to create an auto-generating truth table. I was curious to find best way to parse something like a truth statement for variables and operators.</p>
<p>I found the solution was using an iterative function which finds the "least significant operator" to split the left and right sides into a smaller subproblem. I created a set of rules to find the least significant operator, as well as a set of rules to find valid versus invalid statements.</p>