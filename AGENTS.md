## How the crew is formed
Two native worker sub-agents live in `agents/`: **`implementer`** and **`test-author`**. The
orchestrator composes a roster then dispatches BOTH concurrently (both `Agent` tool calls in one
turn), exactly mirroring neuron's `asyncio.gather` over its workers — one orchestrator, parallel
worker sub-agents.
