# Development Log

## Instructions
Document your development process as you work on the assignment. Add entries showing:
- What you worked on
- Problems you encountered
- How you solved them
- Time spent

**Requirements**: Minimum 5 entries showing progression over time.

---

## Example Entry Format:

### Entry 1 - [April 1, 2026, 2:30 PM]
**What I did**: Forked the repository and set up my student ID

**Details**: 
- Created GitHub account with university email
- Forked the starter repository
- Changed student ID on line 92 to my actual ID (441234567)
- Compiled and ran the program successfully

**Challenges**: Had to install JDK first because javac wasn't recognized

**Solution**: Downloaded JDK 17 from Oracle website and set PATH variable

**Time spent**: 30 minutes

---

## Your Development Log:

### Entry 1 - [march 25,2026,4:00 Pm]
**What I did**: Started the assignment and set up the project.

**Details**:
  •	Downloaded the starter code
	•	Opened project in IDE
	•	Changed student ID in the code
	•	Ran the program to understand output

**Challenges**: 
Didn’t fully understand how threads were being used in the simulation.
**Solution**: Reviewed how Runnable and Thread work and traced execution step by step.

**Time spent**: 45 minutes

---

### Entry 2 - [March 26, 2026, 6:30 PM]
**What I did**: 
Worked on implementing process priority.
**Details**: 
  •	Added priority field to Process class
	•	Modified constructor to include priority
	•	Generated random priority values (1–5)
	•	Displayed priority when adding to queue
**Challenges**: 
Making sure priority is stored and printed correctly for each process.
**Solution**: 
Used getter method and tested output multiple times.
**Time spent**:1 hour 

---

### Entry 3 - [March 27, 2026, 8:00 PM]
**What I did**: 
Implemented context switch counter.

**Details**: 
  •	Added static counter in SchedulerSimulation
	•	Incremented counter each time a new process starts
	•	Printed total at end of simulation

**Challenges**: 
Understanding where exactly to increment the counter.
**Solution**: 
Placed it inside the main scheduling loop before starting each thread
**Time spent**: 40 minutes 

---

### Entry 4 - [March 28, 2026, 9:15 PM]
**What I did**: 
Implemented waiting time tracking.
**Details**: 
  •	Added fields: creationTime, totalWaitingTime, lastReadyTime
	•	Created methods to update waiting time
	•	Calculated waiting time before each execution
	•	Updated ready time when re-queued

**Challenges**: 
Getting correct waiting time calculation without errors.
**Solution**: 
Used System.currentTimeMillis() and tested with multiple runs.
**Time spent**:  1.5 hours

---

### Entry 5 - [March 29, 2026, 10:30 PM]
**What I did**: 
Created summary table for processes.
**Details**: 
  •	Stored completed processes in list
	•	Printed table with process name, burst time, priority, waiting time
	•	Calculated average waiting time

**Challenges**: 
Formatting output to look clean and readable.

**Solution**: 
Used String.format and adjusted spacing.

**Time spent**: 1 hour

---

### Entry 6 - [March 30, 2026, 11:45 PM]
**What I did**: 
Final testing and improvements.

**Details**: 
	•	Tested full simulation multiple times
	•	Verified all features work together
	•	Cleaned up code and comments
	•	Improved output formatting

**Challenges**: 
Minor bugs with queue display and formatting.

**Solution**: 
Debugged step by step and fixed print logic.

**Time spent**: 50 minutes

---

## Summary

**Total time spent on assignment**: [6 hours]

**Most challenging part**: Implementing accurate waiting time calculation and tracking it across queue cycles.

**Most interesting learning**: Understanding how CPU scheduling works using Round Robin with threads.

**What I would do differently next time**: Plan the structure earlier and test each feature separately before combining everything.

