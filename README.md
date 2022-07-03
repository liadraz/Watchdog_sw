# Watchdog_sw
A program that checks that a given client-process is running. In case of an error or a malfunction in the client-process the watchdog responsible for recover it.


### Motivation for using a WatchDog
Watchdogs are commonly found in many systems where humans cannot easily access the equipment or would be unable to react to faults in a timely manner. In such systems, the computer cannot depend on a human to invoke a reboot if it hangs; it must be self-reliant.

The current Project provides an API `./include/watchdog.h` with two main functions: run or stop watching. The user can run the watchdog whenever he decides; in a critical section or for a longer durations.


### WD API Design
The program includes the following modules
Public to the user
- watchdog.h

Private modules
- keep_watching.h
- scheduler.h

<img src="https://github.com/liadraz/Watchdog_sw/blob/main/docs_info/modules.png?raw=true" align="center">




## Usage
Download the following repo in order to use the watchdog.
Run `make` cmd to build all the necessary files.

```bash
    make watchdog
```

Output files: `libwd.so` `run_wd.out`.

* Make sure both files exists in your main program directory.



## Tests
See `./test` directory.

