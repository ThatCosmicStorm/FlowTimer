# FlowTimer
## Basic Idea
- Based on Flowtime and Pomodoro techniques.
- Keeps track of how long you focus on something and gives a set amount of break time.
## Instructions for use
- To start a focus session, press ENTER
- The time you spend in each focus session is noted
- To end the current focus session, press ENTER again
- The break length is mainly based on the length of the focus session (see Default parameters)
- To start your break, press ENTER
- When the break is over, you are prompted to begin another focus session
- Typing Q and pressing ENTER ends the script, giving you the total time (if any) spent in focus sessions and breaks
## Philosophy
- FlowTimer is mainly based on the Flowtime technique, with a slight influence from the Pomodoro technique
- Flowtime lets you work for as long as you want, giving you a specific break time based on how long you worked
## Default parameters
### Break time
- If you worked for less than 10 minutes, you take a 1-minute break.
    - $x<10\qquad y=1$
- If you worked for 10 minutes or more but less than 25 minutes, you take a 5-minute break.
	- $10\le x<25\qquad y=5$
- If you worked for 25 minutes or more but less than 50 minutes, you take a 10-minute break.
	- $25\le x<50\qquad y=5$
- If you worked for 50 minutes or more but less than 90 minutes, you take a 15-minute break.
	- $50\le x<90\qquad y=5$
- If you worked for more than 90 minutes, you take a 20-minute break.
	- $90\le x\qquad y=20$
### Pomodoro influence
- After completing four consecutive focus sessions, your break time is tripled only for the associated break
	- $y=y*3$