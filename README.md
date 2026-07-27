# iyf-s11-week-06-alianjiku-cmd
ynchronous programming was devised to accommodate for the lag between when a function is called to when the value of that function is returned.


Lesson 11 Tasks


**Daily Challenges**
 *Day 1: Delayed Promise task.*
It uses setTimeout wrapped in a Promise so you can await it.                                                                                                                        Task 11.1: Understanding Async 

Day 2: Promise Chain
 
** Sample Output**
1. First resolved after 1482 ms
2. Second resolved after 2765 ms
3. Third resolved after 1910 ms
4. Total Execution Time: 6.16s
5. All promises completed!**
 
 **How it Works**
-random Promise() creates a promise that resolves after a random delay between 1 and 3 seconds.
-first(), second(), and third() each return one of these promises.
-The promises are chained using .then(), so each starts only after the previous one finishes.
-console.time () and console.timeEnd() measure the total time taken for the entire chain.
