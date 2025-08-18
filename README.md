
**This is the official course website for TTM4205 Secure Cryptographic Implementations during Fall of 2025.**

This course was taught for the first time during the fall semester of 2023. The course material and assignments from earlier semesters can be found here: [2023](https://tjerandsilde.no/TTM4205/2023) and [2024](https://tjerandsilde.no/TTM4205/2024). Furthermore, the grade distribution in this course can be found at [karakterer.net/course/TTM4205](https://karakterer.net/course/TTM4205), and I encourage you to check out the student evaluations from [2023](evaluation/2023.pdf) and [2024](evaluation/2024.pdf).

<base target="_blank" >

## Course Description

*The course covers how to implement, analyse, attack, protect and securely compose cryptographic algorithms in practice.  
It goes in depth on how to implement computer arithmetic, attacking implementations using side-channel attacks and fault  
injection, exploit padding oracles and low-entropy randomness, utilise techniques to defend against these attacks, and how  
to securely design misuse-resistant APIs.*

See the full course description at [ntnu.edu/studies/courses/TTM4205](https://www.ntnu.edu/studies/courses/TTM4205).

## Course Staff

Lecturer: &ensp;                    Tjerand Silde  
Contact:  &ensp;&nbsp;              [tjerand.silde@ntnu.no](mailto:tjerand.silde@ntnu.no)  
Office:   &ensp;&ensp;&ensp;&nbsp;  [Electro B225](https://link.mazemap.com/F1ujWlEP)  
Webpage:  &nbsp;                    [tjerandsilde.no](https://tjerandsilde.no)

Lab/Teaching Assistant:             Caroline Sandsbråten  
Contact:  &ensp;&nbsp;              [caroline.sandsbraten@ntnu.no](mailto:caroline.sandsbraten@ntnu.no)  
Office:   &ensp;&ensp;&ensp;&nbsp;  [Electro B211](https://link.mazemap.com/DBIM3jA0)  
Webpage:  &nbsp;                    [carosa.no](https://carosa.no)

## Reference Group

Please reach out to be involved in the reference group.

<!--

The reference group consist of the following members:

  - Adrian Tokle Storset (adriats), from MSTCNNS
  - Daniel Nils Braun (danienbr), exchange student
  - Jiaqi Chen (jiaqic), from SECCLO
  - Emil Bragstad (emil.bragstad), from MTKOM

Reference group meetings: 

- Monday September 23rd: [minutes](minutes/2024/sept-23.pdf)
- Monday October 21st: [minutes](minutes/2024/oct-21.pdf)
- Monday December 9th: [minutes](minutes/2024/dec-09.pdf)

-->

## Ed Forum

We use Ed as a forum in this course, and enrolled students can access the forum at [edstem.org/eu/courses/2376](https://edstem.org/eu/courses/2376).  
Note that the first time you log in to Ed you must do so using the link in the sidebar on Blackboard.

## Course Materials

The course materials are the lecture slides, references therein, and the assignments.  
We do not require that you buy any books, but recommend the following literature:

  1. *Serious Cryptography* by Jean-Philippe Aumasson at [akademika.no](https://www.akademika.no/teknologi/data-og-informasjonsteknologi/serious-cryptography-2nd-edition/9781718503847)
  2. *Real-World Cryptography* by David Wong at [akademika.no](https://www.akademika.no/teknologi/data-og-informasjonsteknologi/real-world-cryptography/9781617296710)

Additional great resources in applied cryptography are:

  - *A Graduate Course in Applied Cryptography* by Dan Boneh and Victor Shoup at [toc.cryptobook.us](https://toc.cryptobook.us) (freely available)
  - *Introduction to Modern Cryptography* by Jonathan Katz and Yehuda Lindell at [akademika.no](https://www.akademika.no/realfag/matematikk/introduction-modern-cryptography/9780815354369) or [NTNU University Library](https://bibsys-almaprimo.hosted.exlibrisgroup.com/permalink/f/11qff65/BIBSYS_ILS71538829360002201)  
  - *The Hardware Hacking Handbook* by Jasper van Woudenberg and Colin O'Flynn at [akademika.no](https://www.akademika.no/teknologi/data-og-informasjonsteknologi/hardware-hacking-handbook/9781593278748)

## Portfolio Assignment

The evaluation in this course will consist of **three** assignments of 100 points total.  

All assignments must be submitted via Ovsys2 at: [ovsys.iik.ntnu.no](https://ovsys.iik.ntnu.no).

### Weekly Problems (40 points)

This assignment will contain the following kinds of problems:

  - Mathematical problems
  - Coding problems
  - [CryptoHack](https://cryptohack.org) problems

The assignement is available here: [TTM4205 Weekly Problems](assignments/2025/Weekly_Problems.pdf) (published 15/8)

The submission deadline is <font color='red'>December 7th at 23:59</font>.

### ChipWhisperer Lab (20 points)

This assignment will contain side-channel attack (SCA) lab work using the [ChipWhisperer Husky](https://rtfm.newae.com/Capture/ChipWhisperer-Husky)  
equipment, which we will provide to all students who signed up for the course. You will get  
access to the CRYPTO-LAB in [Electro A176](https://link.mazemap.com/nYuDTF8q) to work on the assignment.

The problem set will be available in September.

<!--

The assignement is available here: [TTM4205 ChipWhisperer Lab](assignments/2024/ChipWhisperer_Lab.pdf) (updated 16/10)

-->

The submission deadline is <font color='red'>December 7th at 23:59</font>.

### Technical Essay (40 points)

This assignment is to write a technical essay about a topic not covered by the  
lectures or to cover a topic from the lectures in more depth. It is mandatory for  
each group to present their work, but it does not count towards the final grades.

*Most important guidelines:*

  - Groups of 2 or 3 students each
  - Essays of roughly 8 to 10 pages
  - Essays written in LaTeX
  - Short oral presentations

The assignement is available here: [TTM4205 Technical Essay](assignments/2025/Technical_Essay.pdf) (published 15/8)

*Deadlines:*

  - Topic/scope/group approval (mandatory, email):  **October 31st**
  - Short oral presentations (mandatory):           **November 17th** or **November 21nd**
  - Draft submission for feedback (voluntary):      **November 21nd**
  - Receive feedback on draft (voluntary):          **December 5th**
  - Final submission (mandatory): <font color='red'>December 19th at 23:59</font>.

### Grading

We will use the [official NTNU grading scale](https://i.ntnu.no/wiki/-/wiki/English/Grading+scale+using+percentage+points) to assign combined grades.

## Lecture Plan

We have the following sessions in [lecture room R73](https://link.mazemap.com/lbXvvRov) this semester:

* Mondays at 15:15-17:00: <font color='blue'>Lecture</font>
* Fridays at 12:15-14:00: <font color='blue'>Lecture</font> *OR* <font color='orange'>Lab</font>
* Fridays at 14:15-16:00: <font color='orange'>Exercises</font> *OR*  <font color='orange'>Lab</font> 

<!--

Guest Lectures in November:

1. **Tuesday 12/11**: Håkon Jacobsen (Thales Norway) on "FPGAs and Cryptography"
2. **Friday 15/11**: Hans Heum (NTNU) on "Quantum Computers and Cryptography"

-->

(the schedule might be subject to small changes)

| Week | Date  | Format                                    | Responsible | Topic                             | Resources                                                                        |
|------|-------|-------------------------------------------|-------------|-----------------------------------|----------------------------------------------------------------------------------|
| 34   | 18/8  | <font color='blue'>Lecture</font>         | Tjerand     | Course Introduction               |                                                                                  |
| 34   | 22/8  | <font color='blue'>Lecture</font>         | Tjerand     | Randomness 1: Entropy             |                                                                                  |
| 34   | 22/8  | <font color='orange'>Exercises</font>     | Caroline    | Exercise Class                    |                                                                                  |
| 35   | 25/8  | <font color='blue'>Lecture</font>         | Caroline    | Randomness 2: Breaking ECDSA      |                                                                                  |
| 35   | 29/8  | <font color='blue'>Lecture</font>         | Tjerand     | Randomness 3: Randomization       |                                                                                  |
| 35   | 29/8  | <font color='orange'>Exercises</font>     | Caroline    | Exercise Class                    |                                                                                  |
| 36   | 1/9   | <font color='blue'>Lecture</font>         | Tjerand     | Legacy Crypto 1: Crypto Wars      |                                                                                  |
| 36   | 5/9   | <font color='blue'>Lecture</font>         | Tjerand     | Legacy Crypto 2: Attacks on TLS   |                                                                                  |
| 36   | 5/9   | <font color='orange'>Exercises</font>     | Caroline    | Exercise Class                    |                                                                                  |
| 37   | 8/9   | <font color='blue'>Lecture</font>         | Tjerand     | Padding Oracles 1: CBC and SHA    |                                                                                  |
| 37   | 12/9  | <font color='blue'>Lecture</font>         | Tjerand     | Padding Oracles 2: RSA Encryption |                                                                                  |
| 37   | 12/9  | <font color='orange'>Exercises</font>     | Caroline    | Excercise Class                   |                                                                                  |
| 38   | 15/9  | <font color='blue'>Lecture</font>         | Tjerand     | Quantum-Safe Encryption           |                                                                                  |
| 38   | 19/9  | <font color='blue'>Lecture</font>         | Tjerand     | Quantum-Safe Signatures           |                                                                                  |
| 38   | 19/9  | <font color='orange'>Lab</font>           | Caroline    | Exercise Class                    |                                                                                  |
| 39   | 22/9  | <font color='blue'>Lecture</font>         | Tjerand     | Side-Channel Attack (SCA): Intro  |                                                                                  |
| 39   | 26/9  | <font color='orange'>Lab</font>           | Caroline    | SCA Setup Tutorial                |                                                                                  |
| 39   | 26/9  | <font color='orange'>Lab</font>           | Caroline    | SCA Lab 1 (2h)                    |                                                                                  |
| 40   | 29/9  | <font color='blue'>Lecture</font>         | Tjerand     | SCA on Symmetric Key Crypto       |                                                                                  |
| 40   | 3/10  | <font color='orange'>Lab</font>           | Caroline    | SCA Lab 2 (4h)                    |                                                                                  |
| 41   | 6/10  | <font color='blue'>Lecture</font>         | Caroline    | SCA on Public Key Crypto          |                                                                                  |
| 41   | 10/10 | <font color='orange'>Lab</font>           | Caroline    | SCA Lab 3 (4h)                    |                                                                                  |
| 41   | 13/10 | <font color='blue'>Lecture</font>         | Tjerand     | SCA on Quantum-Safe Crypto        |                                                                                  |
| 42   | 17/10 | <font color='orange'>Lab</font>           | Caroline    | SCA Lab 4 (4h)                    |                                                                                  |
| 43   | 20/10 | <font color='blue'>Lecture</font>         | Tjerand     | Crypto API Failures               |                                                                                  |
| 43   | 24/10 | <font color='blue'>Lecture</font>         | Tjerand     | Commitments and Zero-Knowledge    |                                                                                  |
| 43   | 24/10 | <font color='orange'>Exercises</font>     | Caroline    | Exercise Class                    |                                                                                  |
| 44   | 27/10 | <font color='blue'>Lecture</font>         | Tjerand     | Protocol Composition 1: RSA       |                                                                                  |
| 44   | 31/11 | <font color='red'>No Class</font>         |             |                                   |                                                                                  |
| 45   | 3/11  | <font color='blue'>Lecture</font>         | Tjerand     | Protocol Composition 2: DLOG      |                                                                                  |
| 45   | 7/11  | <font color='blue'>Lecture</font>         | Tjerand     | Course Summary                    |                                                                                  |
| 45   | 7/11  | <font color='orange'>Exercises</font>     | Caroline    | Exercise Class                    |                                                                                  |
| 46   | 10/11 | <font color='purple'>Guest Lecture</font> | Tjerand     | Guest Lecture 1                   |                                                                                  |
| 46   | 14/11 | <font color='purple'>Guest Lecture</font> | Tjerand     | Guest Lecture 2                   |                                                                                  |
| 46   | 14/11 | <font color='orange'>Exercises</font>     | Caroline    | Exercise Class                    |                                                                                  |
| 47   | 17/11 | <font color='purple'>Presentations</font> | Tjerand     | ***Project Presentations***       |                                                                                  |
| 47   | 21/11 | <font color='purple'>Presentations</font> | Tjerand     | ***Project Presentations***       |                                                                                  |
| 47   | 21/11 | <font color='orange'>Exercises</font>     | Caroline    | Exercise Class                    |                                                                                  |
