# job-format.md

A job is written by the plan session and handed over whole, in one block. It says five things.

```
WHY
Where this comes from, in the client's or the user's own words if there are any.

WHAT IS ALREADY ESTABLISHED
File and line for each fact. Marked: verify each before you build.

CHANGES
What to change, where. One purpose per job.

NOT IN THIS JOB
What must not be touched. The invariants. Written every time, even when it seems obvious.

VERIFY
How we will know it worked: the cases to run, what to look at, in which environment.
Then the report: done, proof, next.
```
