## How the crew is formed
The orchestrator composes the roster; **each worker is then dispatched by the coordinator as its
OWN separate session** (the `neuron-worker` agent), and the workers run **concurrently** — 1:1
with neuron, which dispatches each worker as its own `ClaudeSDKClient` session under `asyncio.gather`.
There are no in-process sub-agents here.
