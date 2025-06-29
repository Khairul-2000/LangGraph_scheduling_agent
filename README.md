# 🚀 Project Management Agent using LLM and LangGraph

In this project, I’m working on the idea of automating **Project Management** using the power of **LLM (Large Language Models)**. The main goal is to reduce the manual effort and save time in planning and scheduling. I'm also using the **LangGraph** framework to design the agent workflow, which is more structured and reliable.

---

## 🧠 How It Works

The agent system is designed as a **graph with three nodes**, where each node has a specific job.

### 1. PlannerAgent
This is the first step of the graph. It takes the project description and breaks it down into **main phases** and **detailed tasks**. Basically, it creates a full plan based on what the project is about.

### 2. SchedulerAgent
Once the plan is ready, this agent assigns a **timeline**, adds **team members** to tasks, and shows **dependencies** between tasks. It works only with the given team members and also chooses a project leader from them.

### 3. ReviewerAgent
This final node checks the full schedule. It finds if there’s anything missing, any unrealistic timelines, or if someone is overloaded. If everything looks good, it says so — otherwise, it gives suggestions.

---

## 🔧 Tech Stack

- **LangGraph** – for managing the flow between agents.
- **LLM (OpenAI or similar)** – for generating smart planning, scheduling, and reviewing outputs.
- **Python** – for writing the logic and connecting everything.

---

## 📥 Input & 📤 Output

- You provide:
  - Project Type
  - Project Objectives
  - Industry
  - Team Members
  - Any additional info needed

- The system gives:
  - 📌 **Project Plan**: Clean list of phases and tasks
  - 🗓️ **Project Schedule**: Timeline with assigned team and dependencies
  - ✅ **Reviewer Feedback**: Suggestions or approval of the plan

---

## 🧩 Agent Graph

Below is the graph that shows how the agents are connected and the flow of the process:

![agent_graph](https://github.com/user-attachments/assets/7a7aca5c-2afe-433f-84fa-ab8cf1cd1e61)


---

