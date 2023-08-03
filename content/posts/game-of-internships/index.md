---
title: "Game of Internships"
date: 2023-07-31T15:37:28+05:30
tags: [On-Campus, Internship, Microsoft, DSA, Projects]
cover:
    image: "battle.jpg"
    relative: true
---

**(unfiltered thoughts ahead)**

The following is story of how I secured my first industrial internship.

## The Coding Rounds

It all started on 22 July 2023 when I had 4 coding rounds scheduled for the day. The companies were JP Morgan (SDE), Google, Sprinklr and DE Shaw (in order). I was feeling lucky that day since I cracked all 4 shortlists. (not really, Google did not shortlist me even after solving both the problems in online test, *its her loss :*)

Next day, I got sore throat and a runny nose along with headache thanks to peak monsoon, which meant bad luck. I had around 4 tests scheduled for 23 July especially Uber and Rubrik! Rubrik came for campus hiring for the first time afaik. I really wanted to try for Rubrik though they had the toughest test ever. Rubrik’s OA had 4 problems (all four were easily 2000+ rated problems or LC *ultra* -Hard). Hence, I did not stand a chance. On the other hand, Uber OA was conducted on CodeSignal and let me tell you, CodeSignal sucks! First of all, Institute Wifi fails with too many nodes so I had to give most of my tests on personal hotspot. However, it too fails during web-cam proctored tests like Uber’s. What followed was 1 hour of continuous logouts and lagging. I barely submitted one solution at the last minute.

Following morning I had Microsoft’s OA. I barely slept through the night before. After having a bad luck a day before, I gathered whatever little hope I could and went to ABLT4 to give Microsoft’s OA at 6 am. They gave us 2 DSA problems to solve under 2 hr on Codility platform — 

*1. Given a 2xN matrix filled with characters ‘R’, ‘W’ and ‘?’, find minimum moves to achieve perfection. To make a move, replace any ‘?’ with ‘R’ or ‘W’. Perfection is such that, for any column (or any row), count of ‘R’ and ‘W’ in the column (or row) is same. If impossible, print -1.*

1. *Given a string A of lower-case letters and an array B of length N. Find minimum index i (0 ≤ i < N) such that for each index j (0 ≤ j ≤ i), we insert a ‘$’ at B[i] position in original string A and as a result, each adjacent occurence of same letter in A shall have atleast one ‘$’ between them.*

First problem was implementation and second could be done using binary search on answer of each type of letter in string A. I was able to solve both luckily!

## The Fall

![The fall](https://media.giphy.com/media/MRwlFSybIiAh2/giphy.gif)


Fast forward to 27 July. At around 12 AM, Google rolled out its interview shortlist and my name was not there :( I saw the shortlist in morning and had a major setback. This was totally unexpected from them since I was able to solve both the problems in their OA and was confident to get shortlisted. I called my sister and cried my heart out wondering if it was not enough to solve both the questions then what was? But God had another plan…

Later that evening, I gave Oracle’s OA and decided that I will try my best to get sorted in Oracle since they offered good money along with great PPO success rate. Then came the night of 28 July. All the week 1 companies rolled out their shortlists for interviews. I kept checking for my name. I did not clear any quant firm. However, I managed to get shortlisted in 5 companies namely — JPMC SDE, Microsoft, DE Shaw, Sprinklr and Oracle (oracle’s shortlist came on 29 July). I did not expect such a great shortlisting tbh.

## The Day before final battle

![The Day before final battle](https://media.giphy.com/media/j4pc3j8ksVSz7ufKYR/giphy.gif)

Next day, I tried to revise OS, OOPs, my projects and some DSA problem from InterviewBit. All this was too much to revise under 24 hr considering that I had interviews the very next day! I also had to choose 2 out of 3 companies that I got shortlists in (Microsoft, DE Shaw and Sprinklr all three had their interviews on 29th). Form for filling the 2 preferences had deadline at 11:59 pm. I initially thought of my choices to be Sprinklr and Microsoft but then changed them to Sprinklr and DE Shaw since Microsoft seemed like pure gamble (Engage 22). However, at the last minute, owing to gut feeling I moved Microsoft up and DE Shaw down to 3rd preference. I believed in god’s plan.

## The Battle of Winterfell

![The Battle of Winterfell](https://media.giphy.com/media/3o7qDYNtT3wVzczm8M/giphy.gif)
outputs:
    home:
        - HTML
        - RSS
        - JSON
Enter 29 July. I woke up at 6:30 am. Microsoft’s round 1 was scheduled at 9 am and we had to reach by 8:30 am. I forgot to have my resume printed before interview. Silly me. Called up anand to get it printed and he managed to do it just in time. I reached ABLT at 8:50 am. First thing I observed was that I was part of male minority. Mostly girls came for the interview. I blamed myself for making a mistake to change my preferences at the last minute because I thought Microsoft came for diversity hiring. Anyway, round 1 began at 9:15 am and was finished by 10:20 am. There was a moderator along with a male interviewer. We greeted each other and I was asked to introduce myself. I did not prepare exact intro but had a basic template in mind (who am I? what I do? what are my interests and aspirations?). 

He then asked to give an overview of one of my projects. I chose my DBMS project. He did not ask any question on it and then moved to ask me 2 DSA problems. First was, given 2 numbers well within integer range, find minimum number of changes in first number in its bit representation to reach the second number. Initially, he asked an incomplete question on the same idea. I guess he did not prepare that problem before-hand. I was able to explain my approach to him. Next question was — Find number of trailing-zeros in decimal representation of N!. I knew the optimal mathematical solution in O(log(n)). However, I first offered a brute force solution of O(n + log(n)) which could easily overflow. He told me that we are going to test it on 20! and wanted a better approach. I offered a O(n * log(n)) solution by prime factorizing each number from 1 to n. He asked me to improve it even further by hinting that we can avoid finding prime factors for each number and instead solve for range.

I then slowely started showing him some observations on how we could do divide n by 2 again and again to get freq of 2’s in n!. I kind of streched my solution build-up for too long and the interviewer told me that we had only 5 minutes remaining and wanted a pseudo-code for the algorithm. I quickly wrote my approach and was asked to dry-run the algo. I did and he seemed satisfied. The round completed with me asking a few queries about life at microsoft.

It was 10:20 am, I was informed to urgently reach Library for Sprinklr’s Round 1. I hurried to the venue right after my Microsoft’s round and within a few minutes my round 1 began. The interviewer was a young and humble guy. He asked me for my intro and introduced himself as well and we quickly got along (he sounded like a haryanwi dude 😂). He gave me one DSA problem — *Given an NxM binary grid, find largest rectangle with all bits 1*. I approached the problem with modified area under histogram. We can maintain cumulative sum of 1’s for each column and iterate over base of rectangle from top to bottom row. Then, for each row, we could find answer using monotonic stack of increasing height indices. He asked me if there were any edge cases that my approach misses. I explained how my approach will cover all of them. It took me a while to satisfy him about my approach and eventually he understood. Then round ended with a little chit-chat. Round 2 got scheduled within next few minutes. This time, the interviewer was senior guy in the company but that I got to know when the interview was about to end. Phew!

During the second interview, the interviewer again asked for my intro and then jumped directly into a DSA problem — *Given a positive integer of length N (1 ≤ N ≤ 1e5), find the smallest number that we can reduce it to after deleting atmost K digits (1 ≤ K < N).* This problem was a little new to me though I had some ideas to try. I approached with a brute force O(N \* K) algo which he agreed to but wanted me to improve the time complexity further. He struggled for a few minutes but got nowhere. The interviewer started giving me a few hints. He asked me to observe how the result changed for different values of K. I started noticing a stack-like pattern and was thinking out loud. I then explained that for each increment in value of K, we try to find left-most largest number and delete it. He nodded and asked me how I would code it. However, I had already entered panic-mode and was struggling to connect the dots. Finally, after a few minutes of me getting nowhere, the interview explained the approach. I believe my try deserved partial points (maybe). He then asked me about *LRU Cache — What it is? How can I code it?* I explained it to him and then quickly wrote a pseudo-code for its key functions — *LRU.get(key) and LRU.put(key, value)*. I explained to him the linked-list + hashmap approach. He then asked me the time-complexity of each line of code and I did. He seemed satisfied. I asked if I had any question to which I asked about life at Sprinklr and what he does? I then request for feedback on me. He pointed out that I should write clean code and write self-explaining function names. I explained to him that I will work on it and the interview ended at 12:50 pm. 

I checked my inbox. My microsoft’s round 2 was scheduled at 12:05 pm. I rushed back to ABLT and asked if it could be rescheduled. The TPR told me to wait until 1:30 pm. I did. I kept waiting and waiting. It was almost 2 pm when I again asked them. They told me to wait until 2:30 pm 😖. At around 3 pm, my batchmate came to my desk with a dejected look on his face and said *“Bhai, tumhara Sprinklr me kat-gya!”*. Now this felt exactly how Titanic's Captain felt when their unsinkable fleet hit the iceberg and sank. My heart was sinking. I had been confident that there was a great chance for me in Sprinklr and was expecting for HR round anytime soon. Also, I was about to have my second round at Microsoft when this news came. I felt the whole world around me sinking. However, there was still something echoing in my mind *“time for a clutch!”*  I quickly prepped myself and waited for another hour before my round 2 began. It was 4:20 pm when the TPR told me that my round was scheduled next (ironical timing 😄). The interview began and I felt relieved that they did not ghost me.

This time, there was only one interviewer. She apologized for the delay and introduced herself. She was a humble and joyous person and had 21 years of experience in the industry! She told me that she was involved with the security-front of Microsoft India and had her own team 😮. She was impressed with my resume and told me I had diverse projects 😊. It was followed by her telling me that I was going to be asked questions concerning security aspects of my projects 😟. Some of the questions she asked me — *My intro, How I implemented authentication in my project and the workflow, What is private key and public key, Difference between HTTP and HTTPS, How OS and programs manage memory cleaning, How I would scale my project for increased demands, About MVC pattern, Some design patterns that I knew about — Singleton, And their practical usage, Any new technology that I had my hands-on recently.* I did not know much about some of these questions and tried to explain whatever I knew. She told me to take a note of the things I did not know about and brush-up my knowledge. She was fine with me not knowing much and commended my curious attitude. The round was not long and only went for about 40 min. She asked me if I had any questions for her and I asked her what were her major concerns in security to which she told me how Azure was the back-bone of Microsoft and what were its major day-to-day issues. I then asked a hilarous question — What is the next big thing at Microsoft 😂. She laughed and said that she isn’t Satya Nadela 😄. However, She explained how Microsoft is working on integrating AI into their products. I finally asked about life at Microsoft and their expectations from interns. The round ended on a good note.

## The After-math

![The After-math](https://media.giphy.com/media/cLwKXWR977b892mceS/giphy.gif)

I came back to hostel to see questioning faces asking me how my rounds went. I returned quietly to my room. Then began the longest evening of my life. I was betting on Microsoft. However, owing to my experiences in the last few days, I was not expecting much. Most of the offers were unoffically rolled out already except Microsoft. I waited. I called my sister and recapped on the key-events of the day. She told to not worry and get prepared for Oracle’s interview for the very next day. My whole family kept praying, especially my sister Richa. I kept my mobile phone next to me, waiting for my TPR to call me for any update. 4 pm… 5 pm… 6 pm… 3 hours passed by, still no update…

I had made up my mind to prepare SQL for Oracle interview. I opened my laptop and googled “*SQL interview questions*”. I was about to open the first GFG link for the same when suddenly my mobile phone rang. It was my TPR. I answered the call hoping for something. Her exact words were, “*Bhai sunn !! tera microsoft me hogya!!”.* These words unleashed a spring inside me and I started jumping 😂. I run short on words to describe how I felt at that moment so we’ll skip that part 🙂…. Anyway, I then called Richa didi for the great news and she was overjoyed. She merged our call with Mummy and Papa we shared the happiness at that moment. Anyway, That evening went in celebration. I slept at 2:30 am. Some endings and some new beginnings.

[And that kids, is how I](https://youtu.be/r4g6BheZBSo) secured my intern at Microsoft!

Thanks for reading so far! If you liked my experience do share with your friends. You can connect with me on [LinkedIn](https://www.linkedin.com/in/jaideepsh/) or [Twitter](https://twitter.com/camperjett).

**~JD**