## Theory of Computation(ToC)

Q 1. The **Kleen Star Operations** accepts the following string of finite length over `set A = {0,1} | wheres string s contains 
even number of 0 and 1`
- [ ] A. 01, 0011, 010101
- [ ] B. 0011, 11001100
- [ ] C. ε, 0011, 11001101
- [x] D. ε, 0011, 11001100

[Kleen Star](https://cstaleem.com/kleene-closure-in-toc)

<details>
  <summary> <b> ε, 0011, 11001100 </b> </summary>

<br/>

| String	    | Number of 0s	| Number of 1s | Valid? |
|-------------|---------------|--------------|--------|
| `01`        | 1 (odd)	      | 1 (odd)	     | No     | 
| `0011`	    | 2 (even)	    | 2 (even)	   | Yes    |
| `010101`	  | 3 (odd)	      | 3 (odd)	     | No     |
| `11001100`	| 4 (even)	    | 4 (even)	   | Yes    |
| `ε`	        | 0 (even)	    | 0 (even)	   | Yes    |
| `11001101`	| 3 (odd)	      | 5 (odd)	     | No     |

> `ε` represents the empty string, which contains no symbols.
> - Number of zeros = 0
> - Number of ones = 0
> - Zero is an even number.
> - So, epsilon satisfies the condition.

Which string has an even number of both 0s and 1s?
- [ ] A. 00011
- [ ] B. 001111
- [x] C. 00001111
- [ ] D. 010

</details>
<!--------------------->

---

Q 2. A language for which **DFA** exists is a __________.
- [x] A. **Regular Language**
- [ ] B. Non-Regular Language
- [ ] C. Any language
- [ ] D. Can't be said

<details>
  <summary> <b> DFA = Deterministic Finite Automata </b> </summary>

<br/>

> A language for which a Deterministic Finite Automaton (DFA) exists is called a Regular Language.

A DFA is a finite-state machine used to recognize regular languages.

It consists of:
- A finite set of states.
- An input alphabet.
- A transition function.
- An initial state.
- A set of final (accepting) states.
A DFA reads an input string symbol by symbol and decides whether to accept or reject it.

### Example

Consider the language of all binary strings containing an even number of 0s.

A DFA can recognize this language using two states:

<img width="377" height="292" alt="image" src="https://github.com/user-attachments/assets/6a6de5df-b381-4cb2-b8aa-8de54f78747a" />

- `q0`: Even number of zeros (initial and accepting state).
- `q1`: Odd number of zeros.
- Reading `0` switches between `q0` and `q1`.
- Reading `1` keeps the machine in the same state.
Since a DFA exists for this language, it is regular.


Remember this relationship:
- **DFA -> Regular Language**
- **NFA -> Regular Language**
- **Regular Expression -> Regular Language**
- **Context-Free Grammar -> Context-Free Language**
> **Important: DFA and NFA have equivalent recognition power.**


</details>
<!--------------------->

---

Q 3. Let `u = 0001`, then `uv = 11010001` and `vu = 00011101`. <br/>
Using the given information what is the identity element for the string?
- [ ] A. `u^-1`
- [ ] B. `v^-1`
- [ ] C. `u^-1v^-1`
- [x] D. `ε`

<details>
  <summary> <b> ε </b> </summary>

<br/>

The identity element for string concatenation is the empty string, represented by `ε`

### 1. What is an identity element?

An identity element is an element that does not change another element when an operation is performed.

For string concatenation: `uε = εu = u`

For example:
- `0001` + `ε` = `0001`
- `ε` + `0001` = `0001`
Therefore, `ε` is the identity element.

Important correction in the question

Given:
-`u = 0001`
- The concatenations appear to be reversed.
If `v = 1101`, then:
- `uv = 00011101`
- `vu = 11010001`
The question lists these in the opposite order. This does not change the identity-element answer.

</details>
<!--------------------->

---

Q 4. For a DFA accepting binary numbers whose decimal equivalent is divisible by 3, what are all the possible remainders?
- [ ] A. 0
- [ ] B. 0,2
- [x] C. 0,1,2
- [ ] D. 0,1,2,3

<details>
  <summary> <b> Any number is divided by 3 then either remainder will be 0 or 1 or 2  </b> </summary>

<br/>

When a binary number is divided by 3, the possible remainders are: 0,1,2
Why? <br/>
Because when dividing by 3, a remainder must always be less than the divisor. `0 <= r < 3`

</details>
<!--------------------->

---

Q 5. Minimum numbers of states require to accept strings ends with 101.
- [ ] A. 3
- [ ] B. 2
- [ ] C. 1
- [ ] D. can't be represented.
- [ ] E. 4

<details>
  <summary> <b> length of string(n) + 1 = 4 </b> </summary>

<br/>

The minimum number of states required by a DFA over the binary alphabet {0,1} to accept strings ending with 101 is 4.

The DFA must check whether the last three symbols of the input are exactly 101

| State	| Meaning            |
|-------|--------------------|
| q0	  | No useful match yet|
| q1	  | Matched 1          |
| q2	  | Matched 10         |
| q3	  | Matched 101 - accepting state |

</details>
<!--------------------->

---

Q 6. If NFA of 5 states excluding the initial state is converted into DFA, maximum possible number of DFA is?
- [ ] A. 64
- [ ] B. 32
- [ ] C. 128
- [ ] D. 187

<details>
  <summary> <b> Maximum DFA states = 2ⁿ </b> </summary>

<br/>

The maximum number of states in an equivalent DFA obtained from an NFA with 6 total states is: `2^6 = 64`

> NFA with n states -> Maximum DFA states = 2ⁿ

> The minimum number of DFA states is 1.

</details>
<!--------------------->

---

Q 7. The class of **CFG(context free grammar)** is not closed under
- [ ] A. Concatenation
- [x] B. **Intersection**
- [ ] C. Union
- [ ] D. Repeated concatenation

<details>
  <summary> <b> Intersection </b> </summary>

<br/>

The class of Context-Free Languages (CFLs) is not closed under general intersection.

CFL is closed under:
- Union
- Concatenation
- Kleene Star

CFL is NOT closed under:
- Intersection (general)
- Complement
- Difference

</details>
<!--------------------->

---

Q 8. Which of the following is **Type 1 language or Type 1 grammar**?
- [ ] A. Regular grammar/Regular language
- [ ] B. Context Free Grammar/ Context Free Language
- [x] C. Context Sensitive Grammar/Context Sensitive Language
- [ ] D. Recursive Enumerable

<details>
  <summary> <b> Type 1 -  Context-Sensitive Grammar </b> </summary>

<br/>

| Type	  | Grammar	                  | Language                   |
|---------|---------------------------|----------------------------|
| Type 0	| Unrestricted Grammar	    | Recursively Enumerable     |
| Type 1	| Context-Sensitive Grammar	| Context-Sensitive Language |
| Type 2	| Context-Free Grammar	    | Context-Free Language      |
| Type 3	| Regular Grammar	          | Regular Language           |

<img width="586" height="317" alt="image" src="https://github.com/user-attachments/assets/258eac16-4e56-452a-befb-c3a5c995b4d1" />


</details>
<!--------------------->

---

Q 9. A context free grammar G is in Chomsky normal form if every production is of the form
- [ ] A. `A -> BC or A -> A`
- [x] B. `A -> BC or A -> a`
- [ ] C. `A -> BCa or B -> b`
- [ ] D. None of these

<details>
  <summary> <b> A -> BC or A -> A </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 10. The context free grammar `S -> SS | 0S1 | 1S0 | ε` generates
- [x] A. Equal number of 0's and 1's
- [ ] B. Unequal number of 0's and 1's
- [ ] C. Any number of 0's followed by any number of 1's
- [ ] D. None of these

<details>
  <summary> <b> Equal number of 0's and 1's </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 11. According to Chomsky hierarchy, which of the following is recognized by recursively enumerable language?
- [x] A. Type 0
- [ ] B. Type 1
- [ ] C. Type 2
- [ ] D. Type 3

<details>
  <summary> <b> Type 0 </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 12. Turing Machine can be represented using:
- [ ] A. Transition table
- [ ] B. Transition diagram
- [ ] C. Instruction description
- [x] D. All of these

<details>
  <summary> <b> All of these </b> </summary>

<br/>

</details>
<!--------------------->

Q 12-a. A universal Turing Machine is the one that:
- [x] A. can simulate any other TM
- [ ] B. has finite number of states
- [ ] C. Is not-deterministic
- [ ] D. has unbounded tape only in both directions

 A universal turing machine(UTM) simulates any other TM when given the machine's description and its input. <br/>
 This is the basis of stored-program computing and foundation of computer science.

---

Q 13. The **complement of a language will only be defined** when and only when the _______ over language is defined.
- [x] A. Alphabet
- [ ] B. Word
- [ ] C. String
- [ ] D. Grammar

<details>
  <summary> <b> Alphabet </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 14. The minimum number of productions required to produce a language consisting of palindrome strimg over `Σ = {a,b}`
- [ ] A. 3
- [ ] B. 7
- [x] C. 5
- [ ] D. 6

<details>
  <summary> <b> 5 </b> </summary>

<br/>

```
S -> aSa
S -> bSb
S -> a
S -> b
S -> ε

aba
bab
aa
bb
abba
```

</details>
<!--------------------->

---

Q 15. A grammmar that produces more than one parse tree for the same is called:
- [ ] A. Contiguous
- [x] B. **Ambibguous**
- [ ] C. Unambiguous
- [ ] D. Regular

<details>
  <summary> <b> Ambibguous </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 16. The laguage accepted by **Push down Automaton**
- [ ] A. Recursive Language
- [x] B. Context Free Language
- [ ] C. Linearly Bounded Language
- [ ] D. All of the mentioned

<details>
  <summary> <b> Context Free Language </b> </summary>

<br/>

|   Machine                  | Language                        |
|----------------------------|---------------------------------|
| Push down Automaton(PDA)   | Context Free Language           |
| Linear Bound Automata(LBA) | Context sensitive Language      |
| Turing machine             | Recursively Enumerable Language |
| DFA/NFA                    | Regular Language                |



Operations in Regular languages are closed under: `Complemenet + Intersection + Union + Concatination + Kleen Star + Reverse + Homomorphism + Inverse Homomorphism`

</details>
<!--------------------->

---

Q 17. Which of the following conversion is not possible(algorithmically)
- [ ] A. Regular Grammar to Context-Free grammar
- [x] B. Non-deterministic pushdown automata to Deterministic pushdown automata
- [ ] C. Non-deterministic finite state automata to deterministic finite state automata
- [ ] D. Non-deterministic Turing machine to deterministic turing machine

<details>
  <summary> <b> Non-deterministic pushdown automata to Deterministic pushdown automata </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 18. Which of the following is not a part of **quin-tuple(five tuple)**?
- [ ] A. Input alphabet
- [x] B. Output alphabet
- [ ] C. Initial state
- [ ] D. Transition function

<details>
  <summary> <b> Output alphabet  </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 19. A **DFA can be represented** in the following format
- [ ] A. Transition graph
- [ ] B. Transition Table
- [ ] C. C Code
- [ ] D. All of these

<details>
  <summary> <b> All of these </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 20. A string X is accepted by finite automata if
- [x] A. `δ*(q,x) ∈ A`
- [ ] B. `δ(q,x) ∈ A`
- [ ] C. `δ*(q0,x) ∈ A`
- [ ] D. `δ*(q0,x) ∈ A`
 
<details>
  <summary> <b> δ*(q,x) ∈ A </b> </summary>

<br/>

A finite automaton is a collection of 5-tuple (Q, ∑, δ, q0, F), where:
- Q: finite set of states
- ∑: finite set of the input symbol
- q0: initial state
- F: final state
- δ: Transition function

</details>
<!--------------------->

---

Q 21. State True or False: Every right-linear grammar generates a regular langauge:
- [x] A. TRUE
- [ ] B. FALSE
- [ ] C. May be
- [ ] D. Can't say

<details>
  <summary> <b> True </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 22. Which of the problme are unsolvable?
- [x] A. Halting Problem
- [ ] B. Boolean Satisfying Problem
- [ ] C. Halting Problem and Boolean Satisfiability problem
- [ ] D. None of the above

<details>
  <summary> <b> Halting Problem </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 23. The **Turing Machine** showed that you could use a system to program any arithmetic task
- [ ] A. Binary
- [ ] B. Electo-mechanical
- [ ] C. Recursive
- [ ] D. Semantic

<details>
  <summary> <b> Recursive </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 24. The complement of a language is defined if and only if the alphabet is defined on the language
- [x] A. alphabet
- [ ] B. words
- [ ] C. strings
- [ ] D. grammar

<details>
  <summary> <b> alphabet </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 25. Halting state of turing machine are:
- [ ] A. start and stop
- [x] B. accept and reject
- [ ] C. start and reject
- [ ] D. reject and allow

<details>
  <summary> <b> accept and reject </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 26. Let the word be **`"automata"`**. The total number of states required to recognize the word using DFA would be:
- [x] A. 9 states
- [ ] B. 8 states
- [ ] C. 10 states
- [ ] D. words can't be recognize using DFA

<details>
  <summary> <b> n + 1 states, n = length of string  </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 27. Which of the following is an extension to the basic model of Turing Machine:
- [ ] A. Multi tape Turing machine
- [x] B. Multi head Turing machine
- [ ] C. Non-deterministic Turing machine
- [ ] D. All of above

<details>
  <summary> <b> All of above </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 28. A universal turing machine is a __________.
- [ ] A. Single tape Turing machine
- [ ] B. Two-tape Turing machine
- [x] C. Reprogrammable Turing machine
- [ ] D. All of the above

<details>
  <summary> <b> Reprogrammable Turing machine </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 29. Can a DFA recognizes a palindrome number?
- [ ] A. Yes
- [x] B. No
- [ ] C. Yes, with input alphabet as *
- [ ] D. can't determine

<details>
  <summary> <b> No, because DFA doesn't have memory so not perform any calculation stuff </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 30. Church's Thesis supports _________
- [ ] A. Both TM is a general-purpose computer and TM is an algorithm and vice-versa are correct
- [ ] B. A turing machine is an algorithm and an algorithm  as a turing machine
- [x] C. Turing machine as a general purpose computer system
- [ ] D. None of them is correct

<details>
  <summary> <b>  Turing machine as a general purpose computer system </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 31. Regular Expression for all strings starts with `b` and ends with `bba` is:
- [ ] A. `aba*b*bba`
- [ ] B. `ab(ab)*bba`
- [x] C. `b(a+b)*bba`
- [ ] D. All of the mentioned

<details>
  <summary> <b> b____bba = b(a+b)*bba  </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 32. Which of the following statement is false:
- [ ] A. A recursive language is also a regular language
- [ ] B. A context free language is also a regular language
- [x] C. A context free language is also a recursive enumerable language
- [ ] D. Both A and B

<details>
  <summary> <b> A context free language is also a recursive enumerable language </b> </summary>

<br/>

Understand the **Chomsky hierarchy: `Regular ⊂ Context-Free ⊂ Context-Sensitive ⊂ Recursive`**

<img width="821" height="680" alt="image" src="https://github.com/user-attachments/assets/85d0d3f4-26ca-41b5-a815-b5cd3b4005e7" />

<img width="1047" height="506" alt="image" src="https://github.com/user-attachments/assets/824e6fee-ae2c-4a35-8b94-2c5018a09412" />


</details>
<!--------------------->

Understand the **Chomsky hierarchy: `Regular ⊂ Context-Free ⊂ Context-Sensitive ⊂ Recursive`**

---

Q 33. A regular language over an alphabet is closed under following operations:
- [ ] A. Union
- [x] B. Concatenation
- [ ] C. Kleene*
- [ ] D. All of the mentioned

<details>
  <summary> <b>  </b> </summary>

<br/>

A **regular language** is closed under several operations. This means that when we apply these operations to regular languages, the resulting language is also regular.

<img width="1020" height="530" alt="image" src="https://github.com/user-attachments/assets/570664eb-4b00-4ad9-adcf-b76556eff775" />


</details>
<!--------------------->

**Context-free languages (CFLs)** are not closed under:
- General intersection of two CFLs
- Complement
- Difference
But CFLs are closed under **intersection** with a regular language.

---

Q 34. Which of the following is true for the language: `{a^p | p is a prime}`
- [ ] A. It is regular but not context free
- [x] B. It is neither regular nor context free, but accepted by a Turing Machine
- [ ] C. It is not accepted by Turing Machine
- [ ] D. It is context free but not regular

<details>
  <summary> <b> It is neither regular nor context free, but accepted by a Turing Machine </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 35. The language `L = {0^m 1^m 0^m | m>= 1}` is a 
- [ ] A. Regular language
- [ ] B. Context free language
- [ ] C. Both A and B
- [x] D. None, bcuz It is CSL context sensitive language

In regular language, there is nothing like comparison, bcuz regular languages doesn't have memory.

Only two values a and b then it can be context free which uses one stack, but more than two context sensitive there we use 2 stack so that compare three values.

<details>
  <summary> <b> bcuz more than two values: CSL context sensitive language </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 36. The language recognize by Turing Machine is:
- [ ] A. Context free language
- [ ] B. context sensitive language
- [x] C. recursive enumerable language
- [ ] D. regular language

<details>
  <summary> <b>  recursive enumerable language </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 37. Language of **finite automata** is:
- [ ] A. Type 0
- [ ] B. Type 1
- [ ] C. Type 2
- [x] D. Type 3

<details>
  <summary> <b> Type 3 </b> </summary>

<br/>

<img width="1032" height="480" alt="image" src="https://github.com/user-attachments/assets/519c2e78-40fa-4e3e-b9da-0a1d07b0de2a" />


</details>
<!--------------------->

---

Q 38. Minimum number of states required to recognize an octal number divisible by 3 is/are:
- [x] A. 3
- [ ] B. 4
- [ ] C. 1
- [ ] D. 2

<details>
  <summary> <b> divisible by three means 0,1,2. So total number of states 3 </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 39. PDA can be represented with the help of
- [ ] A. Instantaneous description
- [x] B. Transition diagram
- [ ] C. Transition table
- [ ] D. All of these

<details>
  <summary> <b>  </b> </summary>

<br/>

<img width="1016" height="536" alt="image" src="https://github.com/user-attachments/assets/422e7da2-759f-468a-bd6d-d4f23a77d3aa" />


> - Finite Automaton (FA) -> 5-tuple
> - Pushdown Automaton (PDA) -> 7-tuple
> - Turing Machine (TM) -> commonly represented as a 7-tuple

</details>
<!--------------------->

---

Q 40. Which language is accepted by a Deterministic Finite Automaton(DFA) having a single state that is both intial and final, with self loop on every input symbol?
- [x] A. `E*`
- [ ] B. `E+`
- [ ] C. `{epsilon}`
- [ ] D. `Phie`

<details>
  <summary> <b> All possible strings over the given input alphabet (\(\Sigma^*\)). </b> </summary>

<br/>

<img width="807" height="672" alt="image" src="https://github.com/user-attachments/assets/3b1944c0-a0a7-4341-9009-9aae202fc3b7" />


</details>
<!--------------------->

---

Q 41. A transition table of a DFA specifies
- [ ] A. only final states
- [x] B. state change for each input
- [ ] C. only the input alphabet
- [ ] D. All accepted string

<details>
  <summary> <b>  </b> </summary>

<br/>

A transition table of a DFA specifies the next state for every combination of the current state and input symbol.

<img width="782" height="626" alt="image" src="https://github.com/user-attachments/assets/32a92e0f-ded6-4b0f-87f4-2671df65b0c9" />


</details>
<!--------------------->

---

Q 42. Which statement about regular language is correct?
- [ ] A. They require a stack
- [ ] B. They require a tape
- [ ] C. They require two queue
- [x] D. They can be accepted by a DFA

<details>
  <summary> <b> They can be accepted by a DFA </b> </summary>

<br/>

A regular language is a language that can be accepted by a Finite Automaton (FA), such as:
- DFA (Deterministic Finite Automaton)
- NFA (Nondeterministic Finite Automaton)

A DFA has:
- A finite number of states.
- An input alphabet.
- A transition function.
- No stack or auxiliary tape.

| Option	                        | Explanation |
|---------------------------------|--------------|
| A. They require a stack	        | Stack is associated with PDA, which recognizes CFLs. |
| B. They require a tape	        | Tape is associated with Turing Machines. |
| C. They require two queues	    | Two queues can simulate a Turing Machine; they are not required for regular languages. |
| D. They can be accepted by a DFA|	Correct. DFA recognizes regular languages. |


</details>
<!--------------------->

Remember this association:
| Automaton	        | Memory structure	  | Language class |
|-------------------|---------------------|----------------|
| Finite Automaton	| Finite states only	| Regular        |
| PDA	              | Stack	              | Context-Free   | 
| Turing Machine	  | Infinite tape (unbounded in theory)	| Recursively Enumerable |



---

Q 43. The `E-closure` of a state includes:
- [ ] A. Only finite states
- [ ] B. only initial states
- [x] C. the state itself and reachable states via `e-transition`
- [ ] D. only state reached by input symbols

<details>
  <summary> <b> the state itself and reachable states via `e-transition` </b> </summary>

<br/>

<img width="912" height="636" alt="image" src="https://github.com/user-attachments/assets/5781825a-bb33-4ba4-abaa-e93b0c89b425" />


</details>
<!--------------------->

---

Q 44. Two states of a DFA are equivalent if they:
- [ ] A. have identical names
- [x] B. accept the same set of suffixes
- [ ] C. have equal transition counts
- [ ] D. are both initial states

<details>
  <summary> <b> accept the same set of suffixes </b> </summary>

<br/>

<img width="1000" height="462" alt="image" src="https://github.com/user-attachments/assets/cf4bdca1-9564-47d5-a278-e314895eb03b" />


</details>
<!--------------------->

---

Q 45. Which statement about DFA and NFA is correct?
- [x] A. Both recognize regular languages
- [ ] B. only DFA recognize regular languages
- [ ] C. only NFA recognize finite languages
- [ ] D. Neither recognizes infinite langugages

<details>
  <summary> <b> Both NFA and DFA recognize regular languages </b> </summary>

<br/>

Both DFA (Deterministic Finite Automaton) and NFA (Nondeterministic Finite Automaton) recognize exactly the same class of languages: Regular Languages.

The difference is in how they process input.

| DFA	                                              | NFA                                         |
|---------------------------------------------------|---------------------------------------------|
| Exactly one transition for each state-input pair	| Can have zero, one, or multiple transitions |
| Only one computation path	                        | May have multiple possible paths            |
| No ε-transitions	                                | May allow ε-transitions in ε-NFA            |
| Recognizes regular languages	                    | Recognizes regular languages                |

> Important: **Every NFA can be converted into an equivalent DFA using subset construction.**

<img width="795" height="146" alt="image" src="https://github.com/user-attachments/assets/4a1abc07-c173-4d37-805b-10b8b40d2959" />


</details>
<!--------------------->

---

Q 46. Which operation preserve the class of regular languages?
- [x] A. taking complements
- [ ] B. taking square roots of string
- [ ] C. matching equal numbers of 0's 1's
- [ ] D. requiring balance paranthesis

<details>
  <summary> <b> taking complements, doesn't invovle calculation as regular languages don't have memory </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 47. In which machine does the output depend on the current state and the input symbol?
- [ ] A. DFA
- [ ] B. Moore Machine
- [x] C. Mealy Machine
- [ ] D. ε-NFA

<details>
  <summary> <b> Mealy Machine Output depends on Current state + input </b> </summary>

<br/>

**Mealy Machine vs Moore Machine**
| Feature	          | Mealy Machine	        | Moore Machine      |
|-------------------|-----------------------|--------------------|
| Output depends on	| Current state + input	| Current state only |
| Output function	  | \(\lambda(Q,\Sigma)\)	| \(\lambda(Q)\)     |
| Output shown on	  | Transitions	          | States             |
| Output changes	  | With state or input	  | With state changes |

</details>
<!--------------------->

---

Q 48. Which statement about regular languages is correct?
- [ ] A. They're closed under complement only.
- [ ] B. They can't recognize by finite automata.
- [ ] C. Their emptiness is undecidable
- [x] D. Their equivalence is decidable

<details>
  <summary> <b> Their equivalence is decidable  </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 49. Which regular represents all strings over `E = {0,1}` ending 01?
- [ ] A. `01(0+1)*`
- [x] B. `(0+1)*01`
- [ ] C. `0*1*`
- [ ] D. `(01)*`

<details>
  <summary> <b> (0+1)*01 </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 50. Which operator has the highest precedence in regular expressions?
- [ ] A. union(+)
- [ ] B. concatenation
- [x] C. kleen star*
- [ ] D. All have equal precedence

<details>
  <summary> <b> kleen star* > concatenation > union </b> </summary>

<br/>

</details>
<!--------------------->


---

Q 51. Which algebric identity is valid for regular expressions?
- [x] A. `R + Phie = R`
- [ ] B. `R + epsilon = phie`
- [ ] C. `Rphie = R`
- [ ] D. `R + R = phie`

<details>
  <summary> <b>  R + Phie = R </b> </summary>

<br/>

<img width="507" height="516" alt="image" src="https://github.com/user-attachments/assets/58ba66dc-d2c2-478a-9be7-7c26f2cb9f44" />

<img width="661" height="670" alt="image" src="https://github.com/user-attachments/assets/53beb62b-332f-4cce-915b-4e561d9671f9" />


</details>
<!--------------------->


---

Q 52. Kleen's theorem establishes the equivalence between:
- [ ] A. DFA and NFA
- [ ] B. CFG and Turing Machine
- [ ] C. NFA and LBA
- [x] D. Finite Automata and Regular Expression

<details>
  <summary> <b> Kleen's theorem = equivalence between Finite Automata and Regular Expression </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 53. Consider the grammar `S -> aSb\epslion` which language does it generate?
- [x] A. `{a^n b^n | n>=0}`
- [ ] B. `{a^n b^m | n,m>=0}`
- [ ] C. `{a^n b^2n | n>=0}`
- [ ] D. `{a^2n b^n | n>=1}`

<details>
  <summary> <b> {a^n b^n | n>=0} </b> </summary>

<br/>

```
a S b
  |
a S b
  |
 epsilon
aabb
```

</details>
<!--------------------->


---

Q 54. Which statement about inherently ambiguous context free language is correct?
- [ ] A. They have no grammar
- [ ] B. They are not generated by any CFG
- [x] C. Every CFG for them is ambiguous
- [ ] D. They are always regular language

<details>
  <summary> <b> Every CFG for them is ambiguous </b> </summary>

<br/>

An inherently ambiguous context-free language is a context-free language for which every possible context-free grammar (CFG) generating that language is ambiguous.

In simple words:

Even if we try to write a different CFG for the same language, we cannot eliminate its ambiguity.

What is an ambiguous grammar?

A CFG is ambiguous if at least one string generated by it has:
- More than one distinct parse tree, or
- More than one leftmost derivation, or
- More than one rightmost derivation.

</details>
<!--------------------->

---

Q 55. Which symbol is considered useless in a CFG?
- [ ] A. A symbol that is both reachable and generating
- [x] B. A symbol that is both unreachable and non-generating
- [ ] C. The start symbol in every grammar
- [ ] D. A terminal used in a production

<details>
  <summary> <b>  Dead end symbol </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 56. Which production form is permitted in Chomsky Normal Form(CNF), apart from the special start-symbol exception for epsilon?
- [ ] A. `A -> BC` 
- [ ] B. `A -> BCD`
- [x] C. `AB -> a`
- [ ] D. `A -> aB`

<details>
  <summary> <b> A -> BC </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 57. Consider the following statements regarding **Undecidability** <br/>
Statement I - **The Halting Problem for Turing Machine is undecidable in general** <br/>
Statement II - **The post Correspondance Problem is undecidable in general**
- [x] A. Both Statement I and Statement II are true
- [ ] B. Both Statement I and Statement II are flase
- [x] C. Statement I is true but Statement II is false
- [ ] D. Statement I is false but Statement II is true

<details>
  <summary> <b> Both Statement I and Statement II are true </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 58. Which operation is not generally closed for context free languages?
- [ ] A. Union
- [ ] B. Concatenation
- [x] C. Kleen star*
- [ ] D. Intersection

<details>
  <summary> <b> Intersection </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 59. Which property of a context free language is decidable for a given CFG?
- [x] A. whether the language is empty
- [ ] B. whether the language is inherently ambiguous
- [ ] C. whether two arbitrary CFGs generate the same language
- [ ] D. whether the language is regular

<details>
  <summary> <b> whether the language is empty </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 60. The **pumping lemma** for context-free langauge is primarily used to:
- [ ] A. prove every CFL is regular
- [ ] B. convert every CFG into DFA
- [x] C. prove certain languages are not context free
- [ ] D. eliminate all amibiguity from a CFG

<details>
  <summary> <b> pumping lemma = prove contract | certain languages are not context free </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 61. A **Pushdown Automata(PDA)** differs from a finite automaton mainly because it has:
- [ ] A. two input tapes
- [x] B. an auxiliary stack
- [ ] C. an output printer
- [ ] D. infinite control states

<details>
  <summary> <b> an auxiliary stack </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 62. A two-stack PDA has computational power equivalent to a:
- [ ] A. DFA
- [ ] B. NFA
- [x] C. Turing machine
- [ ] D. Single stack DPDA

<details>
  <summary> <b>  Turing machine </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 63. Which statement correctly distinguish recursive languages from recursively enumerable languages?
- [ ] A. Recursive languages need no Turing machine
- [ ] B. Recursive enumerable languages always halt on every input
- [x] C. Recursive languages have a decider that halts on every input
- [ ] D. Both classes contain only regular languges

<details>
  <summary> <b> Recursive languages have a decider that halts on every input </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 64. The Halting problem for a Turing Machine is: 
- [ ] A. Decidable for every input
- [ ] B. Decidable only for deterministic machines
- [ ] C. Decidable using finite automata
- [x] D. Undecidable in general

<details>
  <summary> <b>  The Halting problem for a Turing Machine is undecidable in general  </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 65. Which statement about the Church Thesis is correct?
- [ ] A. It is formally proved theorem of mathematics
- [ ] B. It states that every problem is decidable
- [x] C. It identifies effectively computable functions with Turing machine
- [ ] D. It states that  every language is regular.

<details>
  <summary> <b> It identifies effectively computable functions with Turing machine </b> </summary>

<br/>

</details>
<!--------------------->



