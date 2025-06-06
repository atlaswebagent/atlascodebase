## Program-for-Thought: Towards Adaptive Planning for Automated Web-Task Completion

<p align="justify"> Large Language Models (LLMs) have shown promise in reasoning and code-related tasks, but they continue to struggle with dynamic software behaviors, especially in Web environments involving interactive Graphical User Interfaces (GUIs). This paper presents ATLAS (Adaptive Task planning & Learning for Automated Surfing), a novel agentic framework designed to enhance LLMs’ Web task-performing capability—enabling them to interpret natural language goals and autonomously interact with Web applications. Unlike prior approaches that lack adaptability and tractability, ATLAS integrates Chain-ofThought (CoT) prompting with a new Program-for-Thought (PfT) strategy, which expresses each reasoning step as executable code for fine-grained verification and backtracking. By combining CoT-based planning, PfT-guided scripting, and multimodal inputs (DOM+screenshots), ATLAS supports adaptive re-planning and precise failure recovery without full-plan regeneration. We demonstrate that ATLAS outperforms state-of-the-art baselines in automated Web testing, offering a more robust, scalable, and user-accessible solution for GUI-based task automation.

### Dataset
The datasets for Atlas have been tested on a subset derived from [WebARena]

├── atlas
│   ├── model
│   │   ├── dataset
│   │   │   ├── low_complexity.json
│   │   │   ├── medium_complexity.json
│   │   │   ├── high_complexity.json
│   │   ├── prompts
│   │   │   ├── planner_instructions.txt
│   │   │   ├── scripter_instructions.txt
│   │   ├── config.yaml
│   │   ├── main.py
│   │   ├── planner.py
│   │   ├── scripter.py
│   │   ├── answering_llm.py
│   └── README.md
