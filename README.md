# Tree-Of-Thoughts-Prompting
This repository provides an implementation of Tree of Thoughts (ToT) prompting using various search algorithms. ToT is a powerful technique for enhancing the reasoning abilities of large language models (LLMs) by decomposing complex problems into intermediate steps and exploring different reasoning paths.

## Algorithms Implemented

The following search algorithms are implemented for ToT:

* **Breadth-First Search (BFS)**: Systematically explores all possible thought paths level by level.
* **Depth-First Search (DFS)**: Explores a single thought path as deeply as possible before backtracking.
* **A\* Search**: A heuristic search algorithm that prioritizes paths based on a cost function.
* **BFS-Heirarchial**: **(Novel Implementation)** An optimized Breadth-First Search algorithm with Heirarchial structure to jump to next depth of the tree if the score evaluated is positive, minimizing further computations and time to process.

**Implementation Details**:

1. **Install Dependencies:**
pip install mistralai

2. **Define Prompt Templates:**
```thought_generation_prompts = [(List of Thought prompts to create a individual thought trees)]```
```evaluation_prompts = [(Your evaluation prompts for each step)]```

## Configuration

* `max_depth`: Maximum depth of the search tree.
* `threshold`: Minimum score for a thought to be considered.
* `number_of_samples`: Number of thought samples to generate at each step.
* `number_of_questions`: Number of questions in the problem.


## Notes

* This implementation uses the `mistralai` library for interacting with the Mistral LLM. You can replace it with your preferred LLM provider.
* You can modify the prompt templates and search parameters to suit your specific problem.

## Copyright Notice
The algorithms implemented in this repository are self-written and subject to copyright. They are provided for educational and research purposes only. Any commercial use or redistribution requires explicit permission from the author.
