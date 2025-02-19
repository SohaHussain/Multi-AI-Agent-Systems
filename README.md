# Multi AI Agent Systems

## Agentic Automation
With the traditional automation, we would write code to automate a process and as the edge cases would start to appear, the code would become more and more complex. At the end, we would end up with a very complex code base with multiple edge cases to cover all the scenarios.

On the other hand, with agentic automations, we can show the options/cases instead of drawing the whole map. 

## AI Agents
With regular prompting with a LLM, we need to interact with it and give it feedback in order to make sure that the LLM produces your desired results.
Although through the interactions with LLM we can get a better result, but we also become a blocker. 

With AI agents, we can break that cycle of continous interactions and allow the LLM to operate autonomously.
In other words, when we get an LLM to engage in their thinking process and ask questions and answer them itself so that it can move on and make better decisions by itself.
One thing that makes these agents super powerful is the ability to use tools. Tools allow the agents to interact with the external world.

## Multi Agent Systems
Multi agent systems grow on top of the agent system, where instead of just having one agent, we have multiple of them. 

For example, if we task an agent with something, that agent can also task another agent with a different problem, providing one single final answer in the end. With the multi agent systems, we an customise a single agent 
to do one task as desired. We can also run each agent on a different LLM. 

## Key Elements of AI Agents
- Role/ Backstory - providing a context to the agent
- Focus - providing specific tools, context, job for the agent to focus on so that it does not hallucinate
- Tools - provide the agent with specific and limited tools to use so that it does not get confused
- Cooperation - take feedback/delegate work from/to other agents to improve their response
- Guardrails - guardrails prevents the agents from derailing and nudge them to stay on track
- Memory - ability of agents to remember its previous actions, learn from it and use that data for new executions

## Key Elements of Agent Tools
Tools allow agents to communicate with the external world 
- Versatile - tool should be able to accept different kinds of request, it needs to be versatile enough to handle the fuzzy inputs of the LLMs
- Fault Tolerant - incase of some failure, the tool should be able to send a message back to the agent so that agent can take some action on it, instead of just stopping the whole process
- Caching  - most of the times, the tool will be communicating with the web through different apis, etc. We have to make sure that the tool takes time to do the request and does not call api for unnecessary requests. So a cackinh layers prevents these unnecessary calls from happening and builds an optimal process. There can be multi agent cache, where if two or more agents are using the same tools with the same arguments, they will be using the caching layer and actually doing an api call. 
