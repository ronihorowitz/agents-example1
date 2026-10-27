# agents-example1

Google Colab notebooks for learning LangGraph.

[Open this branch in Colab](https://colab.research.google.com/github/ronihorowitz/agents-example1/blob/dialogue-state-example/notebooks/agents_example1.ipynb)

Choose **Runtime → Run all** to install LangGraph and verify the imports. This first step needs no API keys or GPU. The installation cell downloads LangGraph and its dependencies into the Colab runtime. Run it again in each fresh runtime.

After setup, the notebook builds a StateGraph with two nodes: add 2, then multiply by 3. It explains shared state, nodes, edges, compilation, and execution, and shows each node's update. Starting with 4 produces 18. No API calls are used.

## Dialogue example on this branch

The same notebook also contains a scripted student/assistant conversation using `add_messages`. It displays the complete dialogue, traces message counts growing from 1 to 4, and compares this with the same graph without a reducer, where only the last message remains. No model or API calls are used. History accumulates within a run; cross-session memory is not configured.
