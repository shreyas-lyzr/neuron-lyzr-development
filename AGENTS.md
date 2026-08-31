## How the crew is formed
The roster is invented at runtime; two reusable worker sub-agents live in `agents/`:
**`implementer`** (writes the code slice) and **`test-author`** (writes the tests). Delegate
to both so each worker's contribution is separately traced, exactly like a real Neuron run.
