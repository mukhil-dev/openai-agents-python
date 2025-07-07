
## OpenAI agents python demo SETUP

1. Set up your Python environment
 Using venv (traditional method)
```bash
python3 -m venv env
source env/bin/activate  
```

2. Install Agents SDK

```bash
pip install openai-agents
```
## Hello world example

```python
from agents import Agent, Runner
#we are importing agent and runner 
agent = Agent(name="Assistant", instructions="You are a helpful assistant")
# creating a agent object
result = Runner.run_sync(agent, "Write a haiku about recursion in programming.")
# creating a runner object
print(result.final_output)
# we print the final output from the runner object

# Code within the code,
# Functions calling themselves,
# Infinite loop's dance.
```

3.Get the OpenAI API key

Get the API Key from OpenAI Platform 
export OPENAI_API_KEY="Enter_your_key_here"

4. Test the agent

