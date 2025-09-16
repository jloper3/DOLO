# DOLO: Declarative Orchestration of LangGraph Agents 🤖

This project is a Python implementation of a supervised "graph of graphs" using **LangGraph**. It creates a multi-agent system where specialized AI agents collaborate to perform complex tasks across the entire software lifecycle, from initial planning and development to production incident response.

This system is built around a hierarchical agent model, featuring a top-level **Orchestrator** for user interaction, a **Workflow Supervisor** for automated processes, and a specialized **SRE Orchestrator** for managing operational incidents.


---

## Core Concepts

* **dolo** uses a structured methodology where different LLM agents are given specific roles, tools, and tasks to mimic a real-world team.
* **Executive Agent:** The primary user-facing agent for **development tasks**. It acts as a command-and-control center, allowing the user to switch between specialists like the `analyst` or `pm`, or to initiate entire development workflows.
* **SRE Agent:** A specialized orchestrator that acts as an **Incident Commander** for **operational tasks**. It manages production incidents by systematically triaging, diagnosing (using specialist tools), and remediating issues.
* **Supervisor Agent:** An automated workflow engine. When a defined workflow is initiated, the Supervisor manages the step-by-step execution, calling each specialist agent in the correct sequence.
* **Easy Custom Config:** Easily create custom agents, tasks, templates and workflows, or use prebuilt components.

---
