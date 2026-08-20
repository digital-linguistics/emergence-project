# emergence-project
An experimental, multi-agent AI architecture using adversarial debate to generate novel ecological solutions
# Emergence Project: Solving the Slow Emergency

> *"I designed this cognitive AI architecture over two half-days because I wanted to find novel solutions for slow emergencies like climate change. It is fully MIT Licensed. Use it, code it, break it, or improve it as you see fit."*

## 1. The Objective
At its core, the Emergence Project is a v0.0 experimental architecture designed to trigger cognitive emergence through forced recursion and multi-agent LLM dialogue.
While it won't single-handedly solve climate change, it serves as an engine to break past standard AI consensus and generate rigorous, out-of-the-box thinking for precise ecological bottlenecks.
Please consider this a foundational work in progress, open for community iteration.

## 2. System Architecture & Rationale
[Paste the Mermaid.js code block here to render the visual flowchart]

### The Core Components
*   **Agent 0 (Semantic Router):** The front gate. It prevents "compute overkill" by instantly answering simple factual queries and only triggering the heavy loop for complex, systemic problems.
*   **Agent 1 (Pragmatic Anchor):** Provides the baseline consensus and acts as the logistical/economic friction during the debate.
*   **Agent 2 (The Kite Complex):** Split into two sub-agents to prevent hallucinations: **2A** generates wild, cross-domain novelty, while **2B** rigorously enforces thermodynamics and a 6-pillar "Eco-logic" checkpoint.
*   **Agent 3 (The Judge):** Evaluates the 10-turn debate transcript against a Semantic Constitution to extract the final actionable blueprint.

## 3. The UI Vision
To minimize cognitive load, the final output must be formatted as a three-column comparative view:
1. **The Consensus Baseline** (The standard industry approach).
2. **The Emergent Solution** (The winning, ecologically validated cross-domain idea).
3. **The Moonshot** (The brilliant failure rejected strictly due to current economic/material bottlenecks).

## 4. The Prompts & The Code
**Where is the code?** 
I am a conceptual AI architect. I have designed the systemic flow, the logic gates, and the core system prompts (located in the `/prompts` folder of this repo). 

I am inviting the open-source community to build the backend. If you are a Python/LangChain developer, feel free to wire up these API loops and bring the Emergence Project to life.

```mermaid
graph TD
    %% Define Node Styles
    classDef user fill:#2d3436,stroke:#dfe6e9,stroke-width:2px,color:#fff
    classDef anchor fill:#0984e3,stroke:#74b9ff,stroke-width:2px,color:#fff
    classDef novelty fill:#6c5ce7,stroke:#a29bfe,stroke-width:2px,color:#fff
    classDef critic fill:#d63031,stroke:#ff7675,stroke-width:2px,color:#fff
    classDef judge fill:#00b894,stroke:#55efc4,stroke-width:2px,color:#fff

    %% Nodes
    A[User Prompt / Problem Statement]:::user
    B[Agent 1: The Anchor <br> Pragmatic Baseline]:::anchor
    
    subgraph The Kite Complex
        C[Agent 2A: Novelty Actor <br> Cross-Domain Generator]:::novelty
        D[Agent 2B: Physics Critic <br> Eco-Logic Filter]:::critic
    end

    E[Agent 3: The Judge <br> Semantic Constitution]:::judge
    F[Final Validated Solution]:::user

    %% Flow Dynamics
    A -->|Initializes| B
    B -->|Provides Standard Solution| C
    
    %% Internal Agent 2 Loop
    C -->|Proposes Emergent Idea| D
    D -.->|Fails Physics/Eco-Check: Refine| C
    
    %% Main Debate Loop
    D -->|Passes Check: Validated Idea| B
    B -.->|Critiques Pragmatism & Logistics| C
    
    %% Handoff to Judge
    B ===>|Turn Limit Reached <br> Passes Transcript| E
    D ===>|Turn Limit Reached <br> Passes Transcript| E
    
    %% Final Output
    E -->|Evaluates vs. Constitution| F
