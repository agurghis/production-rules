# RULES.md

Each rule has one line of why. The longer story behind each one is in The Production Kit: https://alexgurghis.com/kit

## Two sessions
1. **The plan session writes jobs and checks reports. It never writes code.** A session that writes the code and checks its own work will tell you it works.
2. **The code session writes code and reports. It never edits the plan.** Whoever writes the code must not be able to rewrite the task.
3. **The premise of a job is a hypothesis.** The code session checks it first, and stops if it's wrong. In one project it caught six wrong premises in ten jobs.
4. **The human carries every job and every report between the two.** It's slower. That's the point.

## Reports
5. **A report is done, proof, next.** If the proof isn't in the report, the job isn't done.
6. **"Added to the menu" is not proof.** Three jobs in a row edited a file nothing loaded.
7. **Proof is what the commit touched, not what the message says.** A job was tagged done with three files missing from it.
8. **What you haven't seen running doesn't exist.** Reminders reported as finished were never sent, for ten months.

## Numbers
9. **Nothing is a number until it's measured.** No sample produces a total.
10. **A number that asks for action gets recomputed from raw data.** 37% was 6.3%.
11. **Never invent a name, a figure, a command or an address.** Not in code, not in a report, not in a message.

## Testing
12. **Test like the person who will use it.** A real click, through every form. A request sent straight to the server skips the part that breaks.
13. **Verify in the environment that contains the problem.** Three clean local checks, and the site was down.
14. **A new test is red first.** A test that has never failed has not tested anything.

## The server
15. **The human runs everything on the server.** The AI writes the command and explains it. It never gets the password.
16. **One deploy command, the same every time.** Build outside the project, restart only after a build that succeeded, roll back by itself.
17. **Check what is being served, not what the terminal says.** A "deploy" that was old scrollback stayed live for a day.
18. **The watcher lives outside what it watches.** A dashboard can say Healthy while the job it reports on has never run.
19. **Backups have retention, live on another disk, and a restore was tested.** Backups once filled the disk and took the site down.
20. **Development settings don't reach production.** One constant kept a server at 100% for a month.

## Data and secrets
21. **Secrets stay on the server, put there by the human. Never in chat.**
22. **One secret lives in one place.** Two files with the same name and different values cost eleven hours.
23. **The data key is not the session key.** Rotating one must not make the other's data unreadable.
24. **No manual SQL on the live database.** Scripts are read-only until the human adds the flag that lets them write.
25. **Public routes create records. They don't change state.**

## The client
26. **The AI drafts. The human cuts and sends.** First drafts come out too long, too formal or too alarmed.
27. **What you tell the client, you test first.**
28. **Text in the client's voice is the client's decision.** Propose it. Don't ship it and announce it.
29. **Default text may only say what the client's data proves.** No invented teams, reviews or guarantees.
30. **If we caused it, we fix it where we caused it.** The client is never asked to clear a cache.
31. **The AI doesn't decide what is commercial.** Contracts, prices and scope are read and decided by the human, clause by clause.
32. **An estimate goes out before the work, not an invoice after it.** Clients object to surprise more than to price.

## Judgement
33. **A new feature waits for a client who asks for it.**
34. **The first phase buys information, not code.** Validation is paid work, and "don't build it" is a valid result.
35. **Invariants go in the brief.** What must not be touched is written down, every time.
36. **Measure the cause before you write the rule.** A precaution based on an unverified cause creates its own defects.
