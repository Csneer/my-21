# my-21

**21 events. 21 days. A clearer next step.**

[简体中文](README.zh-CN.md) · [English skill](skills/en/my-21/SKILL.md) · [中文技能](skills/zh-CN/my-21/SKILL.md)

my-21 is a small agent skill for seeing your next step in a changing world. It brings together **21 of today's trending events** and **the past 21 days of your digital work** to explore where you may be heading—and which new possibilities are worth choosing.

The interesting connection might be a project whose old blocker has disappeared, an idea that can now use work you have already done, or a good reason to keep following your current plan.

> A good result helps you recognize yourself while seeing a possibility you had not considered.

## Two ways to look ahead

| Perspective | What it helps you see |
| --- | --- |
| **Where you may be heading** | The next actions suggested by your recent work, recurring interests, unfinished tasks, and current commitments. |
| **What becomes worth choosing** | A different next step made possible by a change in the world, considered in the context of your own goals and accumulated work. |

These perspectives belong together. A prediction describes a possible continuation; a suggestion gives you a choice. Taking that suggestion may change what happens next.

## A glimpse of the experience

*The following is a fictional example, not a real prediction or a current news report.*

> **Your recent work:** You are finishing an offline log tool. CSV export is still unfinished. You previously set aside PDF reports because their tables were difficult to parse.
>
> **Today's change:** A local document parser adds support for the table structure that stopped you.
>
> **Where you may be heading:** You will probably keep working toward a small demonstration, starting with the export you have already planned.
>
> **A new possibility:** After that demonstration, the old PDF example may be worth another look. A condition that made the idea impractical has changed; some of your earlier work may now be useful.

The value lies in connecting a specific piece of your history with a specific change outside it. The agent chooses how to express the discovery.

## Install

Each language version is a complete, standalone skill. Both use the name **`my-21`**; choose one language to install.

| Language | Skill folder |
| --- | --- |
| English | [`skills/en/my-21`](skills/en/my-21) |
| 简体中文 | [`skills/zh-CN/my-21`](skills/zh-CN/my-21) |

### With an agent that supports skill installation

Ask your agent:

```text
Install the my-21 skill from the GitHub repository Csneer/my-21,
using the folder skills/en/my-21.
```

For Chinese, use `skills/zh-CN/my-21`. The agent needs access to the repository and a supported skill installation workflow.

### Manually in Codex

Clone the public repository and copy your chosen `SKILL.md` into the user skill directory. No GitHub sign-in is needed:

```bash
git clone https://github.com/Csneer/my-21.git
cd my-21
mkdir -p ~/.agents/skills/my-21
cp skills/en/my-21/SKILL.md ~/.agents/skills/my-21/SKILL.md
```

If you already downloaded or cloned the repository, run only the last two commands from its root. To use Chinese, replace the source path with `skills/zh-CN/my-21/SKILL.md`. The copy installs or updates the chosen version at that destination.

If the new skill does not appear, restart the Codex session. Other agents may use a different skill directory; follow the host's installation instructions.

## Try it

Invoke the installed skill in Codex:

```text
$my-21

Use the project notes and task history I have shared from the past 21 days,
along with 21 of today's trending events, to explore what I might do next
and which different directions are worth considering.
```

You can also give it a more immediate question:

```text
$my-21 Is there anything I put aside recently that today's changes make worth revisiting?
```

```text
$my-21 Which of today's events could change what I am already planning to do?
```

## Give it context it can use

Useful material includes project notes, code activity, selected conversations, tasks, and calendars. Existing statements of what you want to finish, change, or leave alone help the agent interpret those records.

The skill uses the context and tools available to its host. Supply the work material you want it to consider, or make those sources available through your agent's supported connections. Current events likewise require web access or a supplied selection of news.

Installing the skill does not collect past activity, create account connections, or start a background service. Its judgments should reflect the material actually available.

Keep personal work records outside this repository. Before sharing results or opening an issue, remove private conversations, credentials, and information about other people.

**21 is the default observation window.** It is not a scientifically established prediction threshold or a requirement to forecast exactly 21 days into the future.

## A small skill, room to think

The skill gives the agent a point of view: understand what is taking shape in your work, explore changes in the world, and imagine what their intersection might make possible. New findings can revise that initial understanding.

It leaves the choice of tools, promising leads, depth of exploration, and response format to the agent. Imagination stays connected to concrete clues, with observations, guesses, and suggestions made distinguishable to the reader.

Read the [design notes](docs/design.md) for the ideas behind this approach, or open the [skill itself](skills/en/my-21/SKILL.md) to see how little text it takes.
