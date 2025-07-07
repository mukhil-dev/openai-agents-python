
## OpenAI agents python demo SETUP

git clone the openai-agents-python repo

create a parent folder called openai_agent

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
## hello.py example file

```bash
touch hello.py
open hello.py
```

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

# Now click save before closing the file. 
```

3.Get the OpenAI API key
```bash
# Get the API Key from OpenAI Platform 
export OPENAI_API_KEY="Enter_your_key_here"
```

4. Test the agent
```
python3 hello.py
```

This throws me the insufficient quota error

