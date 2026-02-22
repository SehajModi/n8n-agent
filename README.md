# Date Suggestion Agent — n8n Workflow

This is an n8n workflow that replicates a Python-based AI dating agent.
It takes two matched users, calculates the distance between them,
and uses Google Gemini to suggest personalised date ideas.

## How to Use
1. Import `date_agent_workflow.json` into n8n
2. Get a free Gemini API key at https://aistudio.google.com
3. Add your API key to the "Call Gemini LLM" node
4. Hit the webhook with a POST request:

{
  "username": "Alice",
  "budget": 50,
  "time": "evening",
  "specification": "Both enjoy hiking"
}

## Available test users
Alice, Bob, Charlie, Diana, Eve, Frank
(Alice↔Bob and Charlie↔Eve are matched)
