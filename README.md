# fpdoc

A bash script that tells you whether your fingerprint reader can work on Linux, and on most distros sets it up for you.

## Usage
 
```
chmod +x fpdoc
./fpdoc check       # look around, change nothing
./fpdoc setup -n    # dry run, prints the commands it would run
./fpdoc setup       # install, enroll, enable (asks first)
```
