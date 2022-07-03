# Watchdog_sw
A program that checks that a given process is running. In case of an error or a malfunction in the client-process the watchdog responsible of recover it.


### Motivation for WatchDog
" Watchdogs are commonly found in many systems where humans cannot easily access the equipment or would be unable to react to faults in a timely manner. In such systems, the computer cannot depend on a human to invoke a reboot if it hangs; it must be self-reliant. "

> There are many ways to implement a watchdog software.

The current Project provides an API `./include/watchdog.h` with two main functions: run or stop watching. The user can run the watchdog whenever he decides; in a critical section or for a longer durations.


### WD Modules




## Usage
Download the following repo in order to use the watchdog.
Run `make` cmd to build all the necessary files.

```bash
    make watchdog
```

Output files: `libwd.so`, `run_wd.out`.

> Make sure both files exists in your main program directory.



## Tests
See `./test` directory.

