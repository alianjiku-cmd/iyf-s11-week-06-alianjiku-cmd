# iyf-s11-week-06-alianjiku-cmd
ynchronous programming was devised to accommodate for the lag between when a function is called to when the value of that function is returned.


Lesson 11 Tasks

**Task 11.3: Promise Chaining **

Expected Output
All Users:
ID: 1
Name: User 1
Email: user1@example.com
----------------------
ID: 2
Name: User 2
Email: user2@example.com
----------------------
ID: 3
Name: User 3
Email: user3@example.com
----------------------
Explanation
.getUserData(id) returns a promise that resolves with a user object.
.Promise.all([...]) starts all three requests at the same time.
.It waits until all promises resolve.
.The users array contains the results in the same order as the promises were passed (user1, user2, user3).
.If any promise fails, the .catch() block executes.



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

**Day 3: Error Handling**

**How it works:**
. DEFAULT_USER — a fallback object for missing users.
. 404 Handling — if the API returns status === 404, we return the default user instead of throwing.
. Other Errors — if the status is not OK (e.g., 500), we throw an error and catch it.
. Network Failures — caught in the catch block, returning the default user.

**Day 4: Rewrite with Async/Await** 

**Sample Output**
-Fetching data...
(wait 2 seconds)
-Data received!Task completed.

**Explanation**
The callback version requires passing a function that runs after the asynchronous operation completes.
In the rewritten version:
fetchData() returns a Promise.
await fetchData() pauses execution inside the async function until the promise resolves.
The code reads from top to bottom, making it easier to understand and maintain compared to nested callbacks.
