---
name: sprint-planning
description: >
  Plans and runs a short sprint: checks that there is a product vision and a backlog of user stories, orders and picks the stories for the sprint, sets a sprint goal and a timebox, defines what done means, shows the result to a real person in a sprint review, and ends with a retrospective. Use when the user wants to plan a sprint, start a sprint, run a mini-sprint in a workshop or class, or asks "what should we build in this sprint". This skill orchestrates sprint-session, sprint-user-stories and sprint-retrospective.
---

# Sprint Planning

This skill is an orchestrator. It plans a sprint, keeps it small, and closes it with a review and a retrospective. You ask questions, the team answers. You never decide what the team builds.

The default sprint is 20 minutes: 5 minutes to plan, 10 minutes to build and review, 5 minutes for the retrospective. In a mini-sprint the review can be one minute with one person. The user can change the timebox. A real sprint is longer, the steps stay the same.

## Team or alone?

Ask first: "Are you working in a team or alone?" If the user is alone, follow the notes under "Working alone" at each step.

## Step 1: Check the starting point

Ask: is there a product vision and a backlog of user stories?

- If yes, ask the user to share them and continue with Step 2.
- If no, load the skill `sprint-session` first. It runs the Product Vision Canvas, the user stories and the Messaging Canvas. Come back to Step 2 when it is finished.

## Step 2: Order and pick the stories for this sprint

Ask who is the product owner (orders the backlog) and who keeps the time. Show the numbered user stories. Ask the product owner to order them by value for the user, most valuable first. Ask the team to give every story an effort estimate (1, 2, 3, 5, 8, 13, 20). Then ask which stories to take into this sprint, from the top, and add up the points. Take only as many points as the team can build. In a short sprint, three to five stories are plenty, one is fine.

If a story is too big for the timebox, load the skill `sprint-user-stories` and split it into smaller stories. If the stories live on a board, move the chosen ones to "In this sprint".

## Step 3: Set the sprint goal and add the improvement

Add the three improvements from the last retrospective to the sprint as tasks, so they are done and not only discussed.

Then ask for one sentence: "At the end of this sprint, a user can ...". Check that every chosen story supports that goal. Remove the stories that do not.

## Step 4: Define done

For every chosen story, take its acceptance criteria (Given-When-Then). A story is done when its criteria pass. If a story has no criteria, write them first.

## Step 5: Run the sprint

Start the timebox and say how long it is. During the sprint:

- Build one story at a time, in the order the team chose, and move its card to "Doing".
- Show a working result at the end of each story, even a small one, and move it to "Done".
- Write new ideas down for the backlog. Do not add them to this sprint.
- Halfway, stop for one minute and ask: what are we working on, and what is blocking us?

## Step 6: Sprint review

Before the retrospective, show the working result to one person outside the team, ideally a real user. Let them try it. Write down what they do, what they say and what surprised them. Turn the feedback into new stories on the backlog.

## Step 7: Retrospective

In the last minutes, load the skill `sprint-retrospective`. It asks what went well, what did not go well and what to change, and turns the answers into three concrete improvements for the next sprint.

## Working alone

Scrum also works for one person. You are the product owner, the builder and the user, so you wear one hat at a time and say out loud which one:

- **Product owner hat, in planning:** order the stories by value for the user, not by what you like building. Take one to three stories.
- **Builder hat, during the sprint:** have only one story in Doing at a time. Use a visible timer. It is your Scrum Master.
- **User hat, in the review:** look at the result as someone who sees it for the first time.
- **Sprint buddy:** pick a classmate or someone from your standup group. Tell them your sprint goal at the start, and show them the result at the end. A sprint review needs someone outside the team.
- **Retrospective:** do it with your buddy. Each of you says one thing that went well and one thing to change.
- **Estimates:** points are relative to your own speed. After the first sprint, the points you finished are your speed. Plan the next sprint with that number. With points you can draw a burn-down chart. That helps a team, but alone and at AI speed it is often overhead: T-shirt sizes are enough.
- **The goal is a working product increment:** each sprint ends with a working step of the product. What that step is comes from the product vision, so ask: what is the end goal of the sprints?
- **The AI is the facilitator, not the buddy:** it keeps the steps and the time, a person gives the feedback.

## Working with AI agents

When an AI agent builds, the sprint keeps its shape but the weight moves from building to deciding and learning:

- **Review sets the scope:** take only as many stories as you or a real person can review in the sprint, not as many as the agent can build.
- **The story is the prompt:** give the agent the story and its acceptance criteria. Use the criteria to check its work.
- **Keep the backlog where the agent reads it:** `BACKLOG.md` in the project folder is context for every session.
- **The sprint goal keeps the agent in bounds:** new ideas go on the backlog, not into the sprint.
- **Review with a real person every sprint:** building fast without feedback only gets you the wrong thing sooner.
- **The retrospective improves the agent too:** when the agent got something wrong, change `AGENTS.md` or the skill, and make that the action for the next sprint.

## Closing

Present a short summary: the sprint goal, the points planned and the points done, the stories that are done, the stories that are not, the feedback from the review, and the three improvements for the next sprint. Compare the points over several sprints. That is how the team learns how much it can build. Ask whether the team wants to plan the next sprint now.

## Make it your own

The length of each step is a starting point. Change it to fit your team. To change the retrospective questions, edit the skill `sprint-retrospective`.
