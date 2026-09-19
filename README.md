# fpdoc

A bash script that tells you whether your fingerprint reader can work on Linux, and on most distros sets it up for you.

## Usage
 
```
chmod +x fpdoc
./fpdoc check                     # look around, change nothing
./fpdoc setup -n                  # dry run, prints the commands it would run
./fpdoc setup                     # install, enroll, enable (asks first)
./fpdoc enroll                    # shows a numbered list, Enter picks right-index-finger
./fpdoc enroll left-thumb         # skip the menu
./fpdoc list                      # what's enrolled
./fpdoc delete right-thumb        # remove one finger
./fpdoc delete all                # remove all of them, then enroll again
./fpdoc enable                    # turn on fingerprint auth in PAM           
./fpdoc diable                    # turn it off again
```

# Enroll

```
>>>:~/fpdoc$ ./fpdoc enroll
   1) left-thumb
   2) left-index-finger
   3) left-middle-finger
   4) left-ring-finger
   5) left-little-finger
   6) right-thumb
   7) right-index-finger
   8) right-middle-finger
   9) right-ring-finger
  10) right-little-finger
number or name [right-index-finger]: 7
[i] touch or swipe the sensor when asked, a few times
Using device /net/reactivated/Fprint/Device/0
Enrolling right-index-finger finger.
Enroll result: enroll-stage-passed
Using device /net/reactivated/Fprint/Device/0
Listing enrolled fingers:
 - #0: right-index-finger
Verify started!
Verifying: right-index-finger
Verify result: verify-match (done)
```
