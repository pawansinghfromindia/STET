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
  <summary> <b>  </b> </summary>

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
- [ ] A. A -> BC or A -> A
- [x] B. A -> BC or A -> a
- [ ] C. A -> BCa or B -> b
- [ ] D. None of these

<details>
  <summary> <b>  </b> </summary>

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
  <summary> <b>  </b> </summary>

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
  <summary> <b>  </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 12.
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> <b>  </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 13.
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> <b>  </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 14.
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> <b>  </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 15.
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> <b>  </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 16.
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> <b>  </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 17.
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> <b>  </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 18.
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> <b>  </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 19.
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> <b>  </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 20.
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> <b>  </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 21.
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> <b>  </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 22.
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> <b>  </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 23.
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> <b>  </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 24.
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> <b>  </b> </summary>

<br/>

</details>
<!--------------------->

---

Q 25.
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> <b>  </b> </summary>

<br/>

</details>
<!--------------------->
