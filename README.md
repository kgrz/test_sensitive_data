If I commit some sensitive data, and then `git reset` it after realizing
the fact, that commit can still be restored using `git reflog`. This is
a test to see if that part of history persists across remote repos.

Test scenario:

  1. Add sensitive data and commit
  2. Reset that commit
  3. Do a push
  4. Clone in a different folder and see if that gets transferred.
