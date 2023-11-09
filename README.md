
**This will be the official course website for TTM4205 Secure Cryptographic Implementations during Fall of 2023.**

<base target="_blank">

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

Lab/Teaching Assistant:             Jonathan Komada Eriksen  
Contact:  &ensp;&nbsp;              [jonathan.k.eriksen@ntnu.no](mailto:jonathan.k.eriksen@ntnu.no)  
Office:   &ensp;&ensp;&ensp;&nbsp;  [Electro B216](https://link.mazemap.com/G4kcT7sc)  
Webpage:  &nbsp;                    [jonathke.github.io](https://jonathke.github.io)

Substitute Lecturer:                Caroline Sandsbråten  
Contact:  &ensp;&nbsp;              [caroline.sandsbraten@ntnu.no](mailto:caroline.sandsbraten@ntnu.no)  
Office:   &ensp;&ensp;&ensp;&nbsp;  [Electro B211](https://link.mazemap.com/DBIM3jA0)  
Webpage:  &nbsp;                    [ntnu.edu/employees/caroline.sandsbraten](https://www.ntnu.edu/employees/caroline.sandsbraten)

## Reference Group

The reference group consist of the following members:

  - Nimer Amol Singh (nimers) from MSSECCLO
  - Espen Sund (espen.sund) from MSMNFMA
  - Diderik Kramer (diderikk) from MSTCNNS
  - Simen Urnes (simen.urnes) from MTKOM

Reference group meetings:

- Thursday September 21st: [minutes](https://tjerandsilde.no/files/TTM4205-reference-group-meeting-september-21.pdf)
- Tuesday October 31st: [minutes](https://tjerandsilde.no/files/TTM4205-reference-group-meeting-october-31.pdf) 

## Piazza Forum

We will use Piazza as a forum in this course.  
Go to [piazza.com/ntnu.no/fall2023/ttm4205](https://piazza.com/ntnu.no/fall2023/ttm4205).  
The sign-up code is: **3dnp6nmmz59**

## Course materials

The course materials are the lecture slides, references therein, and the assignments.  
We do not require that you buy any books, but can recommend the following literature:

  1. *Serious Cryptography* by Jean-Philippe Aumasson at [akademika.no](https://www.akademika.no/teknologi/data-og-informasjonsteknologi/serious-cryptography/9781593278267)
  2. *Real-World Cryptography* by David Wong at [akademika.no](https://www.akademika.no/teknologi/data-og-informasjonsteknologi/real-world-cryptography/9781617296710)
  3. *The Hardware Hacking Handbook* by Jasper van Woudenberg and Colin O'Flynn at [akademika.no](https://www.akademika.no/teknologi/data-og-informasjonsteknologi/hardware-hacking-handbook/9781593278748)

Additional great resources in applied cryptography are:

  - *A Graduate Course in Applied Cryptography* by Dan Boneh and Victor Shoup at [toc.cryptobook.us](https://toc.cryptobook.us) (freely available)
  - *Introduction to Modern Cryptography* by Jonathan Katz and Yehud Lindell at [akademika.no](https://www.akademika.no/realfag/matematikk/introduction-modern-cryptography/9780815354369) or [NTNU University Library](https://bibsys-almaprimo.hosted.exlibrisgroup.com/permalink/f/11qff65/BIBSYS_ILS71538829360002201)

## Portfolio Assignment

The evaluation in this course will consist of two assignments of 100 points total.

### Weekly problems (40 points)

This assignment will contain the following kind of problems:

  - Pen & paper problems
  - Coding problems
  - CryptoHack problems
  - ChipWhisperer labs

The submission deadline is <font color='red'>December 1st at 23:59</font>.

The problems are available here: [PDF](https://tjerandsilde.no/files/TTM4205_Weekly_Problems.pdf) (updated 2/11)

### Special Topic Project (60 points)

This assignment is to write a paper about either a topic not covered  
by the lectures, or to cover a topic from the lectures more in-depth.

*Most important guidelines:*

  - Groups of 1-3 members
  - Papers of 10-20 pages
  - Papers written in LaTeX
  - Short oral presentations

*Deadlines:*

  - Topic/scope/group approval:     **November 1st**
  - Short oral presentations:       **November 23rd**
  - Draft submission for feedback:  **November 23rd**
  - Receive feedback on draft:      **December 1st**
  - Final submission: <font color='red'>December 22nd at 23:59</font>.

Latex-template for the paper: [overleaf.com/read/nhcnrbnwzmcw](https://www.overleaf.com/read/nhcnrbnwzmcw).  
Latex-template for the presentation: [overleaf.com/read/zjqxggmjnzqp](https://www.overleaf.com/read/zjqxggmjnzqp).

The project description is available here: [PDF](https://tjerandsilde.no/files/TTM4205_Special_Topic_Project.pdf) (published 18/8)

### Grading

You must pass both assignments to pass the course; at least 40% on each.

We will use the [official NTNU grading scale](https://i.ntnu.no/wiki/-/wiki/English/Grading+scale+using+percentage+points) to assign combined grades.

## Lecture Plan

We have the following sessions this semester:

* Tuesdays at 12:15-14:00 in [R92](https://link.mazemap.com/d6jlRO3B): <font color='blue'>Lectures</font>
* Tuesdays at 14:15-16:00 in [R92](https://link.mazemap.com/d6jlRO3B): <font color='red'>Lab Session/Exercises</font>
* Thursdays at 10:15-12:00 in [B3](https://link.mazemap.com/lAdJJfsN): <font color='blue'>Lecture</font> *OR* <font color='red'>Lab/Exercises</font>

Guest Lectures in November:

1. **Tuesday 14/11**: Håkon Jacobsen (Thales Norway) on "FPGAs and Cryptography"
2. **Thursday 16/11**: Oskar Goldhahn (IMF, NTNU) on "Formal Verification"
3. **Tuesday 21/11**: Vadim Lyubashevsky (IBM Zurich) on "Post-Quantum Crypto"

(the schedule will be subject to small changes)

| Week | Date  | Format                              | Responsible | Topic                             | Resources                                                                        |
|------|-------|-------------------------------------|-------------|-----------------------------------|----------------------------------------------------------------------------------|
| 34   | 22/8  | <font color='blue'>Lecture</font>   | Tjerand     | Course Introduction               | [Slides](https://tjerandsilde.no/files/TTM4205-Lecture-1.pdf)                    |
| 34   | 22/8  | <font color='red'>Lab/Ex</font>     | Tjerand     | Assignments & Setup               | [Installation Guide](https://github.com/tjesi/TTM4205/blob/main/CW-Setup.ipynb)  |
| 34   | 24/8  | <font color='blue'>Lecture</font>   | Tjerand     | Randomness 1                      | [Slides](https://tjerandsilde.no/files/TTM4205-Lecture-2.pdf)                    |
| 35   | 29/8  | <font color='blue'>Lecture</font>   | Caroline    | Randomness 2                      | [Slides](https://tjerandsilde.no/files/TTM4205-Lecture-3.pdf)                    |
| 35   | 29/8  | <font color='red'>Lab/Ex</font>     | Caroline    | Randomness Exercises              |                                                                                  |
| 35   | 31/8  | <font color='blue'>Lecture</font>   | Tjerand     | Randomness 3                      | [Slides](https://tjerandsilde.no/files/TTM4205-Lecture-4.pdf)                    |
| 36   | 5/9   | <font color='blue'>Lecture</font>   | Tjerand     | Legacy Crypto 1                   | [Slides](https://tjerandsilde.no/files/TTM4205-Lecture-5.pdf)                    |
| 36   | 5/9   | <font color='red'>Lab/Ex</font>     | Jonathan    | Legacy Crypto Exercises           |                                                                                  |
| 36   | 7/9   | <font color='blue'>Lecture</font>   | Tjerand     | Legacy Crypto 2                   | [Slides](https://tjerandsilde.no/files/TTM4205-Lecture-6.pdf)                    |
| 37   | 12/9  | <font color='blue'>Lecture</font>   | Tjerand     | Side-Channel Attacks 1            | [Slides](https://tjerandsilde.no/files/TTM4205-Lecture-7.pdf)                    |
| 37   | 12/9  | <font color='red'>Lab/Ex</font>     | Jonathan    | SCA Lab 1                         |                                                                                  |
| 37   | 14/9  | <font color='red'>Lab/Ex</font>     | Jonathan    | SCA Lab 2                         |                                                                                  |
| 38   | 19/9  | <font color='blue'>Lecture</font>   | Tjerand     | Side-Channel Attacks 2            | [Slides](https://tjerandsilde.no/files/TTM4205-Lecture-8.pdf)                    |
| 38   | 19/9  | <font color='red'>Lab/Ex</font>     | Jonathan    | SCA Lab 3                         |                                                                                  |
| 38   | 21/9  | <font color='red'>Lab/Ex</font>     | Jonathan    | SCA Lab 4                         |                                                                                  |
| 39   | 26/9  | <font color='blue'>Lecture</font>   | Tjerand     | Side-Channel Attacks 3            | [Slides](https://tjerandsilde.no/files/TTM4205-Lecture-9.pdf)                    |
| 39   | 26/9  | <font color='red'>Lab/Ex</font>     | Jonathan    | SCA Lab 5                         |                                                                                  |
| 39   | 28/9  | <font color='red'>Lab/Ex</font>     | Jonathan    | SCA Lab 6                         |                                                                                  |
| 40   | 3/10  | <font color='blue'>Lecture</font>   | Jonathan    | Side-Channel Attacks 4            | [Slides](https://tjerandsilde.no/files/TTM4205-Lecture-10.pdf)                   |
| 40   | 3/10  | <font color='red'>Lab/Ex</font>     | Jonathan    | SCA Lab 7                         |                                                                                  |
| 40   | 5/10  | <font color='red'>Lab/Ex</font>     | Jonathan    | SCA Lab 8                         |                                                                                  |
| 41   | ~~10/10~~ | ~~<font color='blue'>Lecture</font>~~ | ~~Tjerand~~ | ~~Protocol APIs~~           |                                                                                  |
| 41   | ~~10/10~~ | ~~<font color='red'>Lab/Ex</font>~~   | ~~Tjerand~~ | ~~Protocol Exercises~~      |                                                                                  |
| 41   | 12/10 | <font color='blue'>Lecture</font>   | Tjerand     | Protocols APIs                    | [Slides](https://tjerandsilde.no/files/TTM4205-Lecture-11.pdf)                   |
| 42   | 17/10 | <font color='blue'>Lecture</font>   | Tjerand     | Padding Oracles 1                 | [Slides](https://tjerandsilde.no/files/TTM4205-Lecture-12.pdf)                   |
| 42   | 17/10 | <font color='red'>Lab/Ex</font>     | Jonathan    | API and Padding Exercises         |                                                                                  |
| 42   | 19/10 | <font color='blue'>Lecture</font>   | Tjerand     | Padding Oracles 2                 | [Slides](https://tjerandsilde.no/files/TTM4205-Lecture-13.pdf)                   |
| 43   | 24/10 | <font color='blue'>Lecture</font>   | Tjerand     | Commitments and Zero-Knowledge    | [Slides](https://tjerandsilde.no/files/TTM4205-Lecture-14.pdf)                   |
| 43   | 24/10 | <font color='red'>Lab/Ex</font>     | Jonathan    | Com + ZK Exercises                |                                                                                  |
| 43   | 26/10 | <font color='blue'>Lecture</font>   | Jonathan    | Protocol Composition 1            | [Slides](https://tjerandsilde.no/files/TTM4205-Lecture-15.pdf)                   |
| 44   | 31/10 | <font color='blue'>Lecture</font>   | Tjerand     | Protocol Composition 2            | [Slides](https://tjerandsilde.no/files/TTM4205-Lecture-16.pdf)                   |
| 44   | 31/10 | <font color='red'>Lab/Ex</font>     | Jonathan    | Composition Exercises 1           |                                                                                  |
| 44   | 2/11  | <font color='red'>Lab/Ex</font>     | Jonathan    | Composition Exercises 2           |                                                                                  |
| 45   | 7/11  | <font color='blue'>Lecture</font>   | Tjerand     | Protocol Composition 3            | [Slides](https://tjerandsilde.no/files/TTM4205-Lecture-17.pdf)                   |
| 45   | 7/11  | <font color='red'>Lab/Ex</font>     | Jonathan    | Assignments                       |                                                                                  |
| 45   | 9/11  | <font color='blue'>Lecture</font>   | Tjerand     | Course Summary                    | [Slides](https://tjerandsilde.no/files/TTM4205-Lecture-18.pdf)                   |
| 46   | 14/11 | <font color='orange'>Lecture</font> | Tjerand     | Guest Lecture: Håkon Jacobsen     |                                                                                  |
| 46   | 14/11 | <font color='red'>Lab/Ex</font>     | Tjerand     | Assignments                       |                                                                                  |
| 46   | 16/11 | <font color='orange'>Lecture</font> | Tjerand     | Guest Lecture: Oskar Goldhahn     |                                                                                  |
| 47   | 21/11 | <font color='red'>Lab/Ex</font>     | Jonathan    | Assigments                        |                                                                                  |
| 47   | 21/11 | <font color='orange'>Lecture</font> | Tjerand     | Guest Lecture: Vadim Lyubashevsky |                                                                                  |
| 47   | 23/11 | <font color='blue'>Lecture</font>   | Tjerand     | ***Project Presentations***       |                                                                                  |
