# The design of my-21

[Back to the project](../README.md) · [中文介绍](../README.zh-CN.md)

my-21 gives an agent a way to connect two views: what is changing in the world, and what is taking shape in a person's work. The result should help that person recognize their current direction and discover a possibility they had not considered.

## A perspective the agent can work with

The skill supplies a purpose, a few useful ways of looking, and a standard for a good result. The agent chooses which leads to follow, which tools to use, how far to explore, and how to present what it finds.

This fits a task where several approaches may be useful and the right next step depends on the material. The [Anthropic skill authoring guide](https://platform.claude.com/docs/en/agents-and-tools/agent-skills/best-practices) recommends high-freedom instructions for that kind of work. OpenAI's [discussion of skills and prompts](https://developers.openai.com/blog/rethinking-skills-and-prompts-for-gpt-6-astra) also describes how overly prescriptive instructions can constrain more capable agents. These are design precedents, not evidence that this particular skill improves every model.

## Understanding can change during exploration

The central instruction is:

> Pursue promising leads independently, and let new findings revise your understanding.

An initial reading of someone's work is provisional. Later context may reveal that a recurring topic was a completed review, that a project was deliberately paused, or that a new external capability changes an old obstacle. Each discovery can change what the agent looks for next.

This draws on the interaction between action and observation explored in [ReAct](https://arxiv.org/abs/2210.03629v3), and on the selective use of information described in [context engineering](https://www.anthropic.com/engineering/effective-context-engineering-for-ai-agents). The skill leaves the agent free to organize that interaction; it does not implement a prescribed search algorithm.

## Imagination with something to stand on

The agent is invited to imagine several ways forward and choose the connections that offer the most insight. An existing piece of work might become useful in a new setting. A previously blocked idea might become feasible. A prominent event might leave the current plan entirely unchanged.

The important connection is explainable: the user can see which observations led to a possibility. What the agent observed, what it expects, and what it recommends remain distinguishable in natural language.

## What 21 means

Twenty-one events provide a view of the outside world. Twenty-one days provide a recent view of personal work. They are the skill's chosen observation windows, not a scientifically established forecasting optimum or a requirement to produce 21 recommendations.

The host agent supplies access to current sources and the work material the user makes available. The skill itself contains no collector, background service, account connection, or persistent memory system. Limited material calls for proportionate conclusions.

## Keep the skill small

Each language edition is a complete `SKILL.md`. There are no required scripts or supporting documents. This note is optional reading for people interested in the design; the agent does not need to load it to use the skill.

Changes should earn their place through use: a clearer purpose, a useful way of seeing the material, or a correction to a recurring misunderstanding. The guiding test remains:

> A good result helps the user recognize themselves while seeing a possibility they had not considered.

The design has been explored with synthetic examples. Its forecasting accuracy and benefit in sustained personal use have not been established.
