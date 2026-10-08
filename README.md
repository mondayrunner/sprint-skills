# Sprint Skills

*Claude skills to go from idea to backlog and message, by [Tim van den Bosch](https://www.linkedin.com/in/timvdbosch) (Sitelane).*

Six small skills to prepare and run a sprint: from product idea to backlog, message and retrospective. Three do one job each,
two orchestrators run them in order and one skill runs the retro. They come from a course on prototyping with AI at Unknown University.

## The skills

| Skill | What it does |
|---|---|
| **sprint-product-vision-canvas** | Five swimlanes, from concrete to broad: target group, needs, product, business goals, vision. |
| **sprint-user-stories** | Writes stories ("As a ... I want ... so that ...") with Given-When-Then acceptance criteria, checks their quality, and puts the backlog on a board (`BACKLOG.md` by default). |
| **sprint-messaging-canvas** | Six steps to a message that fits your audience: struggle, solution, hesitations, awareness, differentiators, success. |
| **sprint-session** | Orchestrator: runs the three skills above in order and passes the output of each step to the next. |
| **sprint-retrospective** | Runs a five-minute retro: what went well, what did not, what we change. Ends with one concrete action. |
| **sprint-planning** | Orchestrator: checks the backlog, orders and picks the stories, sets a sprint goal and a timebox, defines done, runs a mid-sprint check and a sprint review with a real person, and ends with a retrospective. Calls sprint-session when there is no backlog yet and sprint-retrospective at the end. |

## Install with your agent (copy and paste)

Paste this into Claude Code, or into any coding agent that can run commands:

```text
Install the skills from https://github.com/mondayrunner/sprint-skills for me.
1. Clone the repo to ~/skills/sprint-skills (or git pull if it is already there).
2. Symlink these folders into ~/.claude/skills: sprint-product-vision-canvas,
   sprint-user-stories, sprint-messaging-canvas, sprint-session,
   sprint-retrospective and sprint-planning.
3. If I use another agent than Claude Code, put them in that agent's skills folder instead.
4. Tell me which skills are installed, then wait.
```

When it is done, start a new session and say: "Run a sprint session for my idea." When you have a backlog: "Plan a 20-minute sprint."

## Install yourself

```bash
mkdir -p ~/skills ~/.claude/skills
git clone https://github.com/mondayrunner/sprint-skills.git ~/skills/sprint-skills
for d in sprint-product-vision-canvas sprint-user-stories sprint-messaging-canvas sprint-session sprint-retrospective sprint-planning; do
  ln -sfn ~/skills/sprint-skills/$d ~/.claude/skills/$d
done
```

No git? Download the [zip](https://github.com/mondayrunner/sprint-skills/archive/refs/heads/main.zip), unzip it, and copy the six `sprint-` folders into `~/.claude/skills`.

To update later: `git -C ~/skills/sprint-skills pull`.

## Make it your own

Skills are plain markdown. Change the questions, add a step, or write your own orchestrator that calls
other skills. Everything in this repo is in English, and the skills answer in English unless you ask for another language.

## License

MIT.

## Credits

The backlog rules, the sprint review and the retrospective follow the ideas of [The Scrum Guide](https://scrumguides.org/) by Ken Schwaber and Jeff Sutherland (CC BY-SA 4.0), rewritten for short sprints in a class.
