# Workflow

**Workflows** follow a fixed set of steps where LLMs and tools are used in a planned way through code.
**Agents**, on the other hand, decide what to do on their own. They choose which tools to use and how to complete tasks without following a strict path.

There are different types of workflows.

### LLM is embedded in predefined code paths

- **Prompt-chaining** is a method where each AI (LLM) call builds on the result of the previous one. It breaks a task into smaller steps, with each step handled one at a time. You can also add checks between steps to make sure everything is going as planned.
- **Parallelization** with LLMs (Large Language Models) means running multiple parts of a task at the same time to work faster or get better results.

### LLM directs control flow through predefined code paths.

It uses a prompt to decide which path to take—like choosing to go left or right—but the options are predefined and do not change.

- **Orchestrator-worker:** In the orchestrator-worker setup, one main LLM (the orchestrator) breaks a task into smaller parts and assigns them to other LLMs (the workers). The orchestrator then collects and combines their responses into a final result
- **Evaluator Optimizer:** In the evaluator-optimizer workflow, one LLM generates a response, and another LLM reviews it and gives feedback in a loop. This process continues until the response improves.
- **Routing** means identifying the type of input and sending it to the right task.