# Results
The result is the same in both implementations. 
Seemingly random numbers are returned. In theory, the answer should be 0, since we want to increment and decrement 1 000 000 times each.
In reality, the scheduler messes with the ordering of different reads/writes, overwriting results from other threads.
