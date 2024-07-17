
**This will be the official course website for TTM4205 Secure Cryptographic Implementations during Fall of 2024.**

This course was taught for the first time during the fall semester of 2023. [The course material and assignments from fall 2023 can be found here](https://tjerandsilde.no/TTM4205/2023). Furthermore, the grade distribution in this course can be found at [karakterer.net/course/TTM4205](https://karakterer.net/course/TTM4205), and I encourage you to check out the [student evaluations from 2023](https://github.com/tjesi/TTM4205/blob/main/evaluation/2023.pdf).

<base target="_blank" >
<style>
link{
    text-decoration: underline;
}
</style>

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

Please get in touch if you want to join the reference group!

## Ed Forum

We will use Ed as a forum in this course. Access to the forum is granted for enrolled students and can be found through the Blackboard sidebar, go to Forum -> Ed Discussion. The forum can also be accessed directly through this link: [edstem.org/eu/courses/1290](https://edstem.org/eu/courses/1290/discussion).

## Course Materials

The course materials are the lecture slides, references therein, and the assignments.  
We do not require that you buy any books, but can recommend the following literature:

  1. *Serious Cryptography* by Jean-Philippe Aumasson at [akademika.no](https://www.akademika.no/teknologi/data-og-informasjonsteknologi/serious-cryptography/9781593278267)
  2. *Real-World Cryptography* by David Wong at [akademika.no](https://www.akademika.no/teknologi/data-og-informasjonsteknologi/real-world-cryptography/9781617296710)
  3. *The Hardware Hacking Handbook* by Jasper van Woudenberg and Colin O'Flynn at [akademika.no](https://www.akademika.no/teknologi/data-og-informasjonsteknologi/hardware-hacking-handbook/9781593278748)

Additional great resources in applied cryptography are:

  - *A Graduate Course in Applied Cryptography* by Dan Boneh and Victor Shoup at [toc.cryptobook.us](https://toc.cryptobook.us) (freely available)
  - *Introduction to Modern Cryptography* by Jonathan Katz and Yehud Lindell at [akademika.no](https://www.akademika.no/realfag/matematikk/introduction-modern-cryptography/9780815354369) or [NTNU University Library](https://bibsys-almaprimo.hosted.exlibrisgroup.com/permalink/f/11qff65/BIBSYS_ILS71538829360002201)

## Portfolio Assignment

The evaluation in this course will consist of **three** assignments of 100 points total.  

All assignments must be submittet via Ovsys2. Submission links will be published later.

### Weekly Problems (40 points)

This assignment will contain the following kinds of problems:

  - Mathematical problems
  - Coding problems
  - CryptoHack problems

The submission deadline is <font color='red'>December 6th at 23:59</font>.

**The problems will be announced here.**

### ChipWhisperer Lab (20 points)

This assignment will contain side-channel attack (SCA) lab work using the ChipWhisperer equipment.

The submission deadline is <font color='red'>December 6th at 23:59</font>.

**The lab work will be announced here.**

### Technical Essay (40 points)

This assignment is to write a technical essay about a topic not covered by the  
lectures or to cover a topic from the lectures in more depth. It is mandatory for  
each group to present their work, but it does not count towards the final grades.

*Most important guidelines:*

  - Groups of 2 students
  - Essays of roughly 8 pages
  - Essays written in LaTeX
  - Short oral presentations

*Deadlines:*

  - Topic/scope/group approval:     **November 1st**
  - Short oral presentations:       **November 19th** or **November 22nd**
  - Draft submission for feedback:  **November 22nd**
  - Receive feedback on draft:      **December 6th**
  - Final submission: <font color='red'>December 20th at 23:59</font>.

The project description is available: [TTM4205_Special_Topic_Project.pdf](assignments/2024/TTM4205_Special_Topic_Project.pdf) (published 17/7)

### Grading

You must pass all assignments to pass the course; at least 40% on each.

We will use the [official NTNU grading scale](https://i.ntnu.no/wiki/-/wiki/English/Grading+scale+using+percentage+points) to assign combined grades.

## Lecture Plan

We have the following sessions in [lecture room B2](https://link.mazemap.com/ib3uHkZX) this semester:

* Tuesdays at 08:15-10:00: <font color='blue'>Lecture</font> *OR* <font color='orange'>Lab</font>
* Fridays at 10:15-12:00: <font color='blue'>Lecture</font>
* Fridays at 12:15-14:00: <font color='orange'>Lab</font> *OR* <font color='orange'>Exercises</font>

Guest Lectures in November:

1. **Tuesday 12/11**: Hans Heum (NTNU) on "Quantum Computers and Cryptography"
2. **Friday 15/11**: Håkon Jacobsen (Thales Norway) on "FPGAs and Cryptography"

(the schedule might be subject to small changes)

| Week | Date  | Format                                    | Responsible | Topic                             | Resources                                                                        |
|------|-------|-------------------------------------------|-------------|-----------------------------------|----------------------------------------------------------------------------------|
| 34   | 20/8  | <font color='blue'>Lecture</font>         | Tjerand     | Course Introduction               |                                                                                  |
| 34   | 23/8  | <font color='blue'>Lecture</font>         | Tjerand     | Randomness 1: Entropy             |                                                                                  |
| 34   | 23/8  | <font color='orange'>Exercises</font>     | Caroline    | Exercises                         |                                                                                  |
| 35   | 27/8  | <font color='blue'>Lecture</font>         | Tjerand     | Randomness 2: Randomisation       |                                                                                  |
| 35   | 30/8  | <font color='blue'>Lecture</font>         | Caroline    | Randomness 3: Breaking ECDSA      |                                                                                  |
| 35   | 30/8  | <font color='orange'>Exercises</font>     | Caroline    | Exercises                         |                                                                                  |
| 36   | 3/9   | <font color='red'>No Class</font>         |             |                                   |                                                                                  |
| 36   | 6/9   | <font color='red'>No Class</font>         |             |                                   |                                                                                  |
| 36   | 6/9   | <font color='red'>No Class</font>         |             |                                   |                                                                                  |
| 37   | 10/9  | <font color='blue'>Lecture</font>         | Tjerand     | Legacy Crypto 1: Crypto Wars      |                                                                                  |
| 37   | 13/9  | <font color='blue'>Lecture</font>         | Tjerand     | Legacy Crypto 2: Attacks on TLS   |                                                                                  |
| 37   | 13/9  | <font color='orange'>Exercises</font>     | Caroline    | Exercises                         |                                                                                  |
| 38   | 17/9  | <font color='orange'>Lab</font>           | Caroline    | SCA Lab 1 (Setup)                 |                                                                                  |
| 38   | 20/9  | <font color='blue'>Lecture</font>         | Tjerand     | Side-Channel Attacks (SCA): Intro |                                                                                  |
| 38   | 20/9  | <font color='orange'>Lab</font>           | Caroline    | SCA Lab 2                         |                                                                                  |
| 39   | 24/9  | <font color='orange'>Lab</font>           | Caroline    | SCA Lab 3                         |                                                                                  |
| 39   | 27/9  | <font color='blue'>Lecture</font>         | Tjerand     | SCA on Symmetric Key Crypto       |                                                                                  |
| 39   | 27/9  | <font color='orange'>Lab</font>           | Caroline    | SCA Lab 4                         |                                                                                  |
| 40   | 1/10  | <font color='orange'>Lab</font>           | Caroline    | SCA Lab 5                         |                                                                                  |
| 40   | 4/10  | <font color='blue'>Lecture</font>         | Caroline    | SCA on Public Key Crypto          |                                                                                  |
| 40   | 4/10  | <font color='orange'>Lab</font>           | Caroline    | SCA Lab 6                         |                                                                                  |
| 41   | 8/10  | <font color='orange'>Lab</font>           | Caroline    | SCA Lab 7                         |                                                                                  |
| 41   | 11/10 | <font color='blue'>Lecture</font>         | Tjerand     | SCA on Post-Quantum Crypto        |                                                                                  |
| 41   | 11/10 | <font color='orange'>Lab</font>           | Caroline    | SCA Lab 8                         |                                                                                  |
| 42   | 15/10 | <font color='blue'>Lecture</font>         | Tjerand     | Padding Oracles 1: CBC and SHA    |                                                                                  |
| 42   | 18/10 | <font color='blue'>Lecture</font>         | Tjerand     | Padding Oracles 2: RSA Encryption |                                                                                  |
| 42   | 18/10 | <font color='orange'>Exercises</font>     | Caroline    | Exercises                         |                                                                                  |
| 43   | 22/10 | <font color='blue'>Lecture</font>         | Tjerand     | Crypto API Failures               |                                                                                  |
| 43   | 25/10 | <font color='red'>No Class</font>         |             |                                   |                                                                                  |
| 43   | 25/10 | <font color='red'>No Class</font>         |             |                                   |                                                                                  |
| 44   | 29/10 | <font color='blue'>Lecture</font>         | Tjerand     | Commitments and Zero-Knowledge    |                                                                                  |
| 44   | 1/11  | <font color='blue'>Lecture</font>         | Tjerand     | Protocol Composition 1: RSA       |                                                                                  |
| 44   | 1/11  | <font color='orange'>Exercises</font>     | Tjerand     | Exercises                         |                                                                                  |
| 45   | 5/11  | <font color='blue'>Lecture</font>         | Tjerand     | Protocol Composition 2: DLOG      |                                                                                  |
| 45   | 8/11  | <font color='blue'>Lecture</font>         | Tjerand     | Course Summary                    |                                                                                  |
| 45   | 8/11  | <font color='orange'>Exercises</font>     | Caroline    | Exercises                         |                                                                                  |
| 46   | 12/11 | <font color='purple'>Guest Lecture</font> | Tjerand     | Guest Lecture 1: Hans Heum        |                                                                                  |
| 46   | 15/11 | <font color='purple'>Guest Lecture</font> | Tjerand     | Guest Lecture 2: Håkon Jacobsen   |                                                                                  |
| 46   | 15/11 | <font color='orange'>Exercises</font>     | Caroline    | Exercises                         |                                                                                  |
| 47   | 19/11 | <font color='purple'>Presentations</font> | Tjerand     | ***Project Presentations***       |                                                                                  |
| 47   | 22/11 | <font color='purple'>Presentations</font> | Tjerand     | ***Project Presentations***       |                                                                                  |
| 47   | 22/11 | <font color='orange'>Exercises</font>     | Caroline    | Exercises                         |                                                                                  |
