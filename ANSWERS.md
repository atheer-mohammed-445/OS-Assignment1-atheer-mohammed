# Assignment Questions

## Instructions
Answer all 4 questions with detailed explanations. Each answer should be **3-5 sentences minimum** and demonstrate your understanding of the concepts.

---

## Question 1: Thread vs Process

**Question**: Explain the difference between a **thread** and a **process**. Why did we use threads in this assignment instead of creating separate processes?

**Your Answer:**

A process is basically a program that is running and has its own memory and resources. A thread is a smaller part inside a process, and multiple threads can run within the same process. The main difference is that processes are heavier and take more time to create, while threads are lighter and share the same memory. In this assignment, we used threads because it’s faster and easier to simulate multiple processes running at the same time. Also, using threads makes it simpler to manage scheduling without creating separate programs. So threads were more practical for this kind of simulation.

---

## Question 2: Ready Queue Behavior

**Question**: In Round-Robin scheduling, what happens when a process doesn't finish within its time quantum? Explain using an example from your program output.

**Your Answer:**

In Round-Robin scheduling, if a process does not finish within its time quantum, it is paused and sent back to the end of the ready queue. This means it will wait for its turn again after the other processes. For example, in my output, I saw a process run for a certain time and then show a message that it still has remaining time. After that, it was added back to the queue and executed again later. This keeps repeating until the process finishes completely. This behavior makes sure that all processes get a fair chance to run.


Example from my output:
```
P1 executed quantum 3000ms
Remaining time: 2000ms
P1 yields CPU for context switch
P1 added to ready queue

```

**Explanation of example:**
[Here, P1 didn’t finish its work, so it used its time quantum and then got moved back to the queue. Later, it will run again when it reaches the front of the queue.


---

## Question 3: Thread States

**Question**: A thread can be in different states: **New**, **Runnable**, **Running**, **Waiting**, **Terminated**. Walk through these states for one process (P1) from your simulation.

**Your Answer:**

[Write your answer here. For each state, explain when P1 enters that state during the simulation. Use your understanding of the code to trace through the lifecycle.]

1. **New**: P1 is in the New state when the thread is created but before it starts running.

2. **Runnable**: After calling start(), P1 becomes ready to run and waits for the CPU.

3. **Running**: P1 is in Running state when the CPU is executing its run() method.

4. **Waiting**:P1 can be in Waiting state when it is sleeping during execution (like using Thread.sleep()), or when it is waiting for its next turn after being re-added to the queue.


5. **Terminated**:P1 reaches Terminated state when it finishes all its remaining time and completes execution.


---

## Question 4: Real-World Applications

**Question**: Give **TWO** real-world examples where Round-Robin scheduling with threads would be useful. Explain why this scheduling algorithm works well for those scenarios.

**Your Answer:**

### Example 1: [Web Browser Tabs]

**Description**: 
[In a web browser, multiple tabs run at the same time and each one needs CPU time.]

**Why Round-Robin works well here**: 
[Round-Robin ensures that each tab gets a fair share of CPU time, so no single tab freezes the browser. It keeps everything responsive and smooth for the user.]

### Example 2: [Operating System Task Scheduling]

**Description**: 
[The operating system manages multiple applications running at the same time, like music, apps, and background processes.


**Why Round-Robin works well here**: 
[Round-Robin helps distribute CPU time fairly between all running programs. This prevents one program from taking all the resources and makes the system feel faster and more balanced.


---

## Summary

**Key concepts I understood through these questions:**
  1.	Difference between threads and processes
	2.	How Round-Robin scheduling works
	3.	Thread lifecycle and states

**Concepts I need to study more:**
  1.	Thread synchronization
	2.	Advanced scheduling algorithms
