# Assignment: Visual Workflow Engine Using React Flow

##  Objective
Design and implement a **component-based visual workflow engine** using **React Flow**.  
The system should allow users to visually create workflows by connecting **JSON-based components**, similar to modern low-code / agent-builder platforms.

The workflow engine must support **pluggable components**, **connectors**, and **data flow orchestration** using JSON input and output contracts.

---

##  Problem Statement
Organizations need flexible automation platforms that integrate with tools like **Google**, **Microsoft**, and **custom APIs**.  
Your task is to build a **visual workflow builder** that allows users to:

- Drag and drop components onto a canvas
- Connect components using input/output ports
- Pass structured JSON data between components
- Execute workflows in a deterministic and validated manner

---

## High-Level Architecture

### Frontend
- **React**
- **React Flow** (workflow canvas)
- Component Palette (left panel)
- Configuration Panel (right panel)

### Backend (.Net)
- **.net Core** 
- Workflow definition storage
- Component execution engine
- Connector abstraction layer
- Save workflow on logical sepration

---

## Component Model

Each component must follow a **standard JSON contract**:

```json
{
  "id": "component-id",
  "type": "input | output | tool | agent | connector | utility",
  "inputs": {},
  "outputs": {}
}
```

## All components must:
- Accept JSON input
- Produce JSON output
- Be connectable to other components

## Required Component Categories
### 1. Input / Output Components

Used to start and end workflows.

#### Examples

- Chat Input
- Text Input
- Webhook nput
- Chat Output
- JSON Output

### Rules

- Input components have output only
- Output components have input only

## Reference
This is how UI should look like, when above assignments done.
<img width="1760" height="992" alt="Screenshot 2026-02-07 at 8 04 01 AM" src="https://github.com/user-attachments/assets/57686b6a-6299-4715-99ee-b3d5af9377b0" />

#### Note
We're not looking whole implimentation (given ref image) but full workflow which shows capabilities. 
