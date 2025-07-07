
## Get started

1. Set up your Python environment
 Using venv (traditional method)
```bash
python -m venv env
source env/bin/activate  
```

2. Install Agents SDK

```bash
pip install openai-agents
```

## Hello world example

```python
from agents import Agent, Runner

agent = Agent(name="Assistant", instructions="You are a helpful assistant")

result = Runner.run_sync(agent, "Write a haiku about recursion in programming.")
print(result.final_output)

# Code within the code,
# Functions calling themselves,
# Infinite loop's dance.
```

Get the API Key from OpenAI Platform 
