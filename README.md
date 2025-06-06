## Program-for-Thought: Towards Adaptive Planning for Automated Web-Task Completion

<p align="justify"> Large Language Models (LLMs) have shown promise in reasoning and code-related tasks, but they continue to struggle with dynamic software behaviors, especially in Web environments involving interactive Graphical User Interfaces (GUIs).

This paper presents **ATLAS** (Adaptive Task planning & Learning for Automated Surfing), a novel agentic framework designed to enhance LLMs’ Web task-performing capability—enabling them to interpret natural language goals and autonomously interact with Web applications.

Unlike prior approaches that lack adaptability and tractability, ATLAS integrates **Chain-of-Thought (CoT)** prompting with a new **Program-for-Thought (PfT)** strategy, which expresses each reasoning step as executable code for fine-grained verification and backtracking.

By combining CoT-based planning, PfT-guided scripting, and multimodal inputs (DOM + screenshots), ATLAS supports adaptive re-planning and precise failure recovery without full-plan regeneration.

We demonstrate that ATLAS outperforms state-of-the-art baselines in automated Web testing, offering a more robust, scalable, and user-accessible solution for GUI-based task automation.

</p>

---

### 📚 Dataset

The datasets used by ATLAS are derived from a subset of **WebArena**, categorized by task complexity:

- `low_complexity.json`
- `medium_complexity.json`
- `high_complexity.json`

---

### 📁 Project Structure
```
├── atlas
│   ├── model
│   │   ├── dataset
│   │   │   ├── low_complexity.json
│   │   │   ├── medium_complexity.json
│   │   │   ├── high_complexity.json
│   │   ├── prompts
│   │   │   ├── planner_instructions.txt
│   │   │   ├── scripter_instructions.txt
│   │   ├── codebase
│   │   │   ├── config.yaml
│   │   │   ├── main.py
│   │   │   ├── planner.py
│   │   │   ├── scripter.py
│   │   │   ├── answering_llm.py
|   └── README.md
```

---

### 🧠 Prompt Instructions

Instruction files guiding different components of the agent:

- `planner_instructions.txt`: Instructions for the planning component
- `scripter_instructions.txt`: Instructions for the scripting component

---

### ⚙️ Core Scripts

- `main.py`: Main entry point to execute tasks
- `planner.py`: CoT-based planner module
- `scripter.py`: PfT-guided scripting module
- `answering_llm.py`: LLM-based reasoning and response handler
- `config.yaml`: Configuration file for experimental setup

---

### 📄 License & Citation

For licensing and citation details, please refer to the accompanying LICENSE file and cite our paper if you use ATLAS in your work.

