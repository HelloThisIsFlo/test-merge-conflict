# test-merge-conflict
SSCCE - Merge Conflict

This is a short example highlighting a point that's unclear to me with 'git merge'

Here are the steps of each commit : 
- A class is created with 2 functions: 'foo' & 'bar'.
- A static variable is added (just to have one more commit before branching)
- A branch is created 'testRemoveBar' in which the 'bar' function is removed, 
  in the meantime in the 'master' branch, a function 'function' is add which depends on function 'bar'
- Finally the two branch are merged.

The problem : 
The two branch are merged without conflict, however the code can't compile anymore.
Indeed in the merged version the function 'bar' has been removed.

Is this a normal behavior ? If so, any tips to avoid this problem ?

Thank you :)
