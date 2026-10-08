---
name: sprint-planning
description: >
  Plans and runs a short sprint: checks that there is a product vision and a backlog of user stories, picks the stories for the sprint, sets a sprint goal and a timebox, defines what done means, and ends with a retrospective. Use when the user wants to plan a sprint, start a sprint, run a mini-sprint in a workshop or class, or asks "what should we build in this sprint". This skill orchestrates sprint-session, sprint-user-stories and the retrospective step.
---

# Sprint Planning

This skill is an orchestrator. It plans a sprint, keeps it small, and closes it with a retrospective. You ask questions, the team answers. You never decide what the team builds.

The default sprint is 20 minutes: 5 minutes to plan, 10 minutes to build, 5 minutes for the retrospective. The user can change the timebox. A real sprint is longer, the steps stay the same.

## Step 1: Check the starting point

Ask: is there a product vision and a backlog of user stories?

- If yes, ask the user to share them and continue with Step 2.
- If no, load the skill `sprint-session` first. It runs the Product Vision Canvas, the user stories and the Messaging Canvas. Come back to Step 2 when it is finished.

## Step 2: Pick the stories for this sprint

Show the numbered user stories. Ask the team which stories to take into this sprint. In a short sprint, three to five stories are plenty, one is fine.

If a story is too big for the timebox, load the skill `sprint-user-stories` and split it into smaller stories.

## Step 3: Set the sprint goal

Ask for one sentence: "At the end of this sprint, a user can ...". Check that every chosen story supports that goal. Remove the stories that do not.

## Step 4: Define done

For every chosen story, take its acceptance criteria (Given-When-Then). A story is done when its criteria pass. If a story has no criteria, write them first.

## Step 5: Run the sprint

Start the timebox and say how long it is. During the sprint:

- Build one story at a time, in the order the team chose.
- Show a working result at the end of each story, even a small one.
- Write new ideas down for the backlog. Do not add them to this sprint.

## Step 6: Retrospective

In the last minutes, ask three questions and write down the answers:

1. What went well?
2. What did not go well?
3. What do we change in the next sprint?

Turn the answer to the third question into one concrete action for the next sprint.

## Closing

Present a short summary: the sprint goal, the stories that are done, the stories that are not, and the action for the next sprint. Ask whether the team wants to plan the next sprint now.

## Make it your own

The questions in the retrospective and the length of each step are a starting point. Change them to fit your team, for example with Start, Stop, Continue instead of the three questions above.
