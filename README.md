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
