# i3blocks-hamster-tracking
A i3blocks integration of the Gnome Time Tracker Project hamster using hamster-cli.

Shows name and duration of currently tracked task as part of your i3blocks bar. Or "Not tracking" if no task is tracked. A second block allows to stop and restart tracking of the last task

### Screenshot while tracking:

![sample records](/tracking.png?raw=true)

Clicking on the clock icon will stop tracking

### Screenshot while not tracking:

![sample records](/not-tracking.png?raw=true)

Clicking on the clock icon will start tracking a new task with the same name and tag as the last one in the hamster list. 

## Sample block config in i3blocks.conf

```
[hamster_pause_resume]
command=/home/user/.i3blocks/hamster_pause_resume
full_text=
separator=false

[hamster_task]
command=/home/user/.i3blocks/hamster_task
interval=60
signal=2
```

**Adjust signal number and amount of days it is looking for tasks in the past to your needs!**
