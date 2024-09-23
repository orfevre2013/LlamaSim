# LlamaPoll - Predict Elections Way Better With LLM Agents

__TLDR: We built a multi-agent framework from scratch and used it to simulate election results in battleground states__ 

Leaner than CrewAI & meaner than Autogen, we easily beat prompting & fine-tuning by using our conversational framework to spawn groupchats of collaborative agents to solve all your problems __(in just 4 lines of code)__.

We adapted this framework to simulate how current events can affect real-time election results: by using census data to replicate voter districts, generating detailed backstories for AI agents, and programming them to think exactly like the voters they are acting out. 
```python
from Network import Network
breaking_news = '''Breaking News! Donald Trump will launch his own cryptocurrency.'''
agent_network = Network(breaking_news, state = "Pennsylvania", num_agents = 15)
agent_network.simulate("round_robin", num_rounds = 1)
