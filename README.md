# TestScript

updated version here: https://github.com/dduan97/testscript_v2/blob/master/ptest

## Features
Bash Script designed to automate testing for simple C programs in CS223 and CS323
Compares the output of the user program with Stan's correct solution.

After every change you can now quickly do regression testing to ensure that no previous
features have been broken by new updates. 

# Usage
1. Install on zoo machine
2. Create a text file of test cases using $PROG to specify user/stan's program.
   e.g. echo aaabbb | $PROG aa a -S0 abb aab -S1
   e.g. $PROG 2 2 5 "abcd" "bca	"
3. Update required path variables at the top of test_script
4. RUN THE SCRIPT! (test_script)

# Additional Flags
-r prints the result output for each test case
-t prints the test cases as they are executed
-n runs only specific test cases
-l adds your time to global leaderboard
   uses only the time to complete public test cases for fairness

## TODO
1. Add flag to test for speed
2. Implement a test for inputs that are designed to 'fail gracefully'
3. Seperate all variables into spec file
