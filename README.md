# Knapsack Problems

> Historical portfolio project. This repository is preserved as an academic artifact and is not actively maintained.

## Overview

This project was completed with a project partner for a Computational Thinking course. It compares two approaches to package selection:

- an exact dynamic-programming solution for the single-knapsack problem;
- a greedy heuristic for the multiple-knapsack problem.

The multiple-knapsack result is intentionally heuristic and is not guaranteed to be globally optimal.

## Repository contents

| Path | Purpose |
| --- | --- |
| `single_knapsack.py` | Dynamic-programming implementation for one knapsack. |
| `multiple_knapsack.py` | Greedy implementation for multiple knapsacks. |
| `data/` | Example CSV inputs used during the project. |
| `CT_Proj.pptx` | Project presentation covering the algorithms and their complexity. |

## Using the code

The Python modules use only the standard library. Their source comments describe the expected package format: `[package_id, reward, weight]`.

```python
from single_knapsack import select_packageSet

packages = [["P001", 8, 4], ["P002", 5, 3], ["P003", 9, 6]]
selected = select_packageSet(10, packages)
```

`select_packageSets` sorts and consumes the list passed to it. Pass a copy if the original list must be retained.

## Attribution and limitations

The dynamic-programming implementation is derived in part from the GeeksforGeeks 0/1 knapsack example credited in the source file. This repository presents coursework, not a maintained optimization library.

## License and reuse

No open-source license has been applied. The project is shared for viewing as portfolio work. Third-party materials remain subject to their respective rights.