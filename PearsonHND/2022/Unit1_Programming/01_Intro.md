# Unit 1 - Programming 

## 1.1 Introduction

- Programming - a technological process for telling a computer which tasks to perform in order to solve problems (analogous to a recipe of a dish)

- Programming Language - a system of notations that is used to compose instruction sets that a computer can understand. A programming language's surface form is known as its [syntax](https://en.wikipedia.org/wiki/Syntax_(programming_languages)). The term [semantics](https://en.wikipedia.org/wiki/Semantics_(computer_science)) refers to the meaning of languages, as opposed to their form (syntax). There are about 9000 different coding languages available, only about 50 of them are the leading contenders.

- High-level vs Low-level Languages
<table>
    <tr>
        <td>Type</td>
        <td>Examples</td>
        <td>Description</td>
        <td>Syntax</td>
    </tr>
    <tr>
        <td>High-level</td>
        <td>Python, VB, Java, C#</td>
        <td>
        	<ul>
        		<li>Independent of hardware (i.e, portable)</li>
        		<li>Translated using compiler/interpreter</li>
        		<li>One statement mostly translates into many machine instructions</li>
        	</ul>
        </td>
        <td>
            <pre lang="python">
a = 10
b = 15
sum = a+b
            </pre>
    	</td>
    </tr>
    <tr>
        <td rowspan="2">Low-level</td>
        <td>Assembly</td>
        <td>
        	<ul>
        		<li>Translated using an assembler</li>
        		<li>One statement translates into one machine instruction</li>
        	</ul>
        </td>
        <td>
        	<pre lang="bash">
LDA181
ADD93
STO185
        	</pre>
        </td>
    </tr>
    <tr>
        <td>Machine Language</td>
        <td>Executable binary code produced by compiler/interpreter/assembler</td>
        <td>
            <pre>
1010000100000111110101
            </pre>
        </td>
    </tr>
</table>

![alt text](00_Src/computer-languages.png "Computer Languages by Level")

- Apart from this, programming languages can be classified into [multiple generations](https://en.wikipedia.org/wiki/Programming_language_generations)

## 1.2. Paradigms

- A programming paradigm is a way to classify programming languages based on their features.
- Paradigms, at a high level, can be classified into two
	- [**Imperative**](https://en.wikipedia.org/wiki/Imperative_programming) - instructs the machine **how** to change its state
	- [**Declarative**](https://en.wikipedia.org/wiki/Declarative_programming) - declares **what** the desired result is (properties of the desired result), but *not how to compute it*

### 1.2.1. Procedural Programming Paradigm

- Set of procedures
- Each procedure defines some functionality (how to do something)
- Procedures are callable/invocable
- E.g. Basic, Pascal, FORTRAN, C

### 1.2.2. Object-Oriented Programming Paradigm

- Comprehend world as a set of objects
- Model each object in computer memory
- Functionality = Interactions between objects
- E.g. C#, Java, Kotlin, Scala, Objective-C, Perl, Python

***
[Home](README.md) | [Next](02_CSBasics.md)