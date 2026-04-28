# Performance-Review
The decision tree is stored in tree/reflection-tree.csv and is structured as a sequence of nodes.

Each row represents a node with the following fields:

id: unique identifier of the node
parent: the node from which it is reached
type: defines behavior (start, question, decision, reflection, bridge, summary, end)
text: content shown to the user
options: possible choices (for questions) or routing logic (for decisions)
target: direct jump to another node (used in bridges/reflections)
signal: tracks user tendencies across axes

The flow begins at start and progresses through:

Axis 1 (Control / Agency)
Axis 2 (Contribution)
Axis 3 (Perspective)

Decision nodes route the flow based on the selected option, ensuring the system remains fully deterministic.
