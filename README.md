# Sprint Skills

*Claude skills to go from idea to backlog and message, by [Tim van den Bosch](https://www.linkedin.com/in/timvdbosch) (Sitelane).*

Six small skills to prepare and run a sprint: from product idea to backlog, message and retrospective. Three do one job each,
two orchestrators run them in order and one skill runs the retro. They come from a course on prototyping with AI at Unknown University.

## The skills

| Skill | What it does |
|---|---|
| **sprint-product-vision-canvas** | Five swimlanes, from concrete to broad: target group, needs, product, business goals, vision. |
| **sprint-user-stories** | Writes stories ("As a ... I want ... so that ...") with Given-When-Then acceptance criteria. |
| **sprint-messaging-canvas** | Six steps to a message that fits your audience: struggle, solution, hesitations, awareness, differentiators, success. |
| **sprint-session** | Orchestrator: runs the three skills above in order and passes the output of each step to the next. |
| **sprint-retrospective** | Runs a five-minute retro: what went well, what did not, what we change. Ends with one concrete action. |
| **sprint-planning** | Orchestrator: checks the backlog, picks the stories, sets a sprint goal and a timebox, defines done and ends with a retrospective. Calls sprint-session when there is no backlog yet and sprint-retrospective at the end. |

## Install

```bash
git clone https://github.com/mondayrunner/sprint-skills.git
cd sprint-skills
for d in sprint-product-vision-canvas sprint-user-stories sprint-messaging-canvas sprint-session sprint-retrospective sprint-planning; do
  ln -s "$(pwd)/$d" ~/.claude/skills/$d
done
```

Then ask Claude: "Run a sprint session for my idea", and when you have a backlog: "Plan a 20-minute sprint."

## Make it your own

Skills are plain markdown. Change the questions, add a step, or write your own orchestrator that calls
other skills. Everything in this repo is in English, and the skills answer in English unless you ask for another language.

## License

MIT.
