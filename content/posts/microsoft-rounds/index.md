---
title: "Microsoft Rounds"
date: 2023-08-01T23:50:17+05:30
tags: [On-Campus, Internship, Microsoft, DSA, Projects]
cover:
    image: "microsoft.jpg"
    relative: true
---

## Coding Round

- The online assessment was hosted on Codility on 24/07/23.
- 2 Programming questions, 110 min total duration.

Q 1. *Given a 2xN matrix filled with characters ‘R’, ‘W’ and ‘?’, find minimum “moves” to achieve “perfection”. To make a move, replace any ‘?’ with ‘R’ or ‘W’. Perfection is such that, for any column (or any row), count of ‘R’ and ‘W’ in the column (or row) is same. If impossible, print -1. [1 ≤ N ≤ 1e5]*

Q 2. *Given a string A of lower-case letters and an array B of length N. Find minimum index i (0 ≤ i < N) such that for each index j (0 ≤ j ≤ i), we insert a ‘$’ at B[i] position (1-indexed) in original string A and as a result, each adjacent occurence of same letter in A shall have atleast one ‘$’ between them. Example:*

*A: abcdacb*

*B: [1, 6, 2, 3]*

*Answer: 2. If i = 0, final string is $abcdacb. If i = 1, final string is $abcda$cb. If i = 2, final string is $a$bcda$cb. As you can see, both the a’s have atleast one $ between them. Same goes for b’s and c’s.*

Approach:

Q1. This was implementation problem. O(n) TC.

Q2. I was able to solve it using binary search. There are many ways to solve it but this is how I solved it — First create a vector of positions for each lower-case alphabet. Then for each alphabet, I would binary search the answer. Afterwards, take maximum of the answer for each alphabet. TC O(M * log(N)) where M: length of string A.

****************************************************************************************************Around 40 students were shortlisted for interview.****************************************************************************************************

## Interview

- Interview was scheduled on 29/07/23 and held online on MS Teams and Codility IDE was used.
- I had 2 interview Rounds (some had 3).
- Rounds were eliminatory in nature.

### Round 1 (Technical)

There was a male interviewer along with a moderator. We greeted each other and I was asked to introduce myself. I did not prepare exact intro but had a basic template in mind (who am I? what I do? what are my interests and aspirations?).

He then asked to give an overview of one of my projects. I chose my DBMS project. He did not ask any question on it and then moved on to ask me 2 DSA problems. 

First was — G*iven 2 numbers well within integer range, find minimum number of changes in first number in its bit representation to reach the second number*. 

Initially, he asked an incomplete question on the same idea. I guess he did not prepare that problem before-hand. I was able to explain my approach to him. 

Next question was — *Find number of trailing-zeros in decimal representation of n!*. 

I knew the optimal mathematical solution in O(log(n)). However, I first offered a brute force solution of O(n + log(n)) which could easily overflow. He told me that we are going to test it on 20! and wanted a better approach. I offered a O(n * log(n)) solution by prime factorizing each number from 1 to n. He asked me to improve it even further by hinting that we can avoid finding prime factors for each number and instead solve over range.

I then slowely started showing him some observations on how we could do divide n by 2 again and again to get freq of 2’s in n!. I kind of streched my solution build-up for too long and the interviewer told me that we had only 5 minutes remaining and wanted a pseudo-code for the algorithm. I quickly wrote my approach and was asked to dry-run the algo on 20!. I did and he seemed satisfied. The round completed with me asking a few queries about life at microsoft.

**Around 7-10 candidates were eliminated after Round 1.**

### Round 2 (Technical)

This time, there was only one interviewer. She introduced herself first and asked me for mine. She was humble and experience of more than 21 years! She told me that she was involved with the security-front of Microsoft India and had her own team. She was impressed with my resume and told me I had diverse projects 😊. It was followed by her telling me that I was going to be asked questions concerning security aspects of my projects. Some of the questions she asked me — *How I implemented authentication in my project and the workflow, What is private key and public key, Difference between HTTP and HTTPS, How OS and programs manage memory cleaning, How I would scale my project for increased demands, About MVC pattern, Some design patterns that I knew about — like Singleton and factory, And their practical usage, Any new technology that I had my hands-on recently.* 

I did not know much about some of these questions and tried to explain whatever I knew. She told me to take a note of the things I did not know about and brush-up my knowledge. She was fine with me not knowing much and commended curious attitude. The round was not too long and only went for about 40 min. She asked me if I had any questions for her and I asked her what were her major concerns in security to which she told me how Azure was the back-bone of Microsoft and what were its major day-to-day issues. I then asked a hilarous question — What is the next big thing at Microsoft 😂. She laughed and said that she isn’t Satya Nadela. However, She explained Microsoft is working on integrating AI into their products at enterprise level. I finally asked about expectations from interns. The round ended on a good note.

**Verdict:** Selected 😇

**Around 10 students were selected**

## General Tips

- Start your interview with a smile and maintain confidence throughout the interview.
- Think of interview as more of a conversation between two people on a DSA problem or some tech.
- Prepare an intro before-hand and keep it short and crisp. Try to mention that you’re looking for a learning opportunity.
- Before answering any question, Take a few moments to think of a structured answer and try to avoid any keyword you do not know much about.
- Avoid faking in resume and write only about the things you know. Same goes for projects mentioned. Interviewers are smart beings and check easily detect if you faked.
- If you do not know the answer, take a small moment to think and then reply with a positive note that you do not know much about it but will be interested in googling up later (note it done on a paper if possible).
- For coding rounds, Start preparing DSA from early on. I started Competitive programming from January 2023 and did DSA during summer vacations for 2 months and was able to get shortlisted in 5 companies in week 1.

Thanks for reading so far. I hope this helped you. All the best\!