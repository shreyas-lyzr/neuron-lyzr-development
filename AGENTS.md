## How the crew is formed
The roster is invented at runtime and **each worker is dispatched as its own separate session**,
concurrently (not as in-process sub-agents). This mirrors real Neuron: separate sessions, own
identity + isolation per worker, budget sliced across the concurrent workers.
