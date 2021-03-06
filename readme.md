berdea
======

Mithat Konar 2014-05-29

Acceptance testing and BDD with bash.

TL;DR
-----
1. Copy the repo into your testing directory
2. Write your behavior tests with files ending with `.test`
    * Use assertions:
        *  `assert/assert` is a low level, general purpose assertion handler.
        * High-level assertions are available in the same directory (needs more!)
    * You can group tests using filterable filenames, e.g. `Eating-a-stick-of-butter.api.test`
3. Specify any setup and teardown you need in the files in `fixtures/`
4. `run-all` will run all the tests (i.e., all the files ending with `.test`) 
   and report pass/fail statuses.
5. You can also write your own  test-runners that execute a subset of all tests 
   by copying `run-all` and
    * explicitly specifying the names of the test files to run in a list, or
    * filtering files by filename, e.g., `for t in $(ls -1 *.api.test) ...`.

Have fun.
