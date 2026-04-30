# Coordinate-Based Memory System (CMS) — Manuscript Abstract

Large language model (LLM) agents increasingly require persistent memory to support long-horizon interaction, user-specific adaptation, and stable behavior across dialogue sessions. Existing approaches typically rely on raw context accumulation, periodic summarization, or retrieval-augmented memory. While useful in practice, these approaches generally treat memory as prompt residue, compressed text, or a query-time retrieval target rather than as an explicitly managed state structure.

We introduce the Coordinate-Based Memory System (CMS), a policy-bounded and explicitly managed memory abstraction for persistent conversational agents. In CMS, memory is organized through a fixed scope-guided partition policy and updated by deterministic insertion, reinforcement, and exposure rules. The present work does not frame CMS as a full cognitive architecture or as a task-optimization method. Instead, it studies whether an explicit state-structured memory mechanism can be defined, implemented, and audited in a reproducible way under long-horizon conversational conditions.

CMS is evaluated against raw context accumulation, summarization-based memory, and retrieval-augmented generation as reference memory paradigms. These baselines anchor CMS against accumulation-, compression-, and similarity-based memory mechanisms. Evaluation focuses on systems-level memory properties, including retention fidelity, contradiction resistance, token footprint, observable update behavior, and bounded processing cost.

Under this framing, lower prompt burden, white-box auditability, selective eviction, and stable retention are treated not as independent headline claims, but as structural consequences of explicit state management. CMS is therefore presented as a minimal, implementation-aligned memory abstraction whose primary contribution lies in validating a distinct design point for persistent conversational memory.

## Status

This is a working manuscript abstract. Final experimental results, citations, and submission formatting are still being completed.


## Figures

### Figure 1. CMS within a modular conversational architecture

<img src="figures/Figure_1_CMS_Modular_Architecture.png" alt="CMS within a modular conversational architecture" width="600">

### Figure 2. Decoupled memory update and generation flow

<img src="figures/Figure_2_Decoupled_Memory_Update_and_Generation_Flow.png" alt="Decoupled memory update and generation flow" width="600">

### Figure 3. Bounded coordinate memory structure

<img src="figures/Figure_3_Bounded_Coordinate_Memory_Structure.png" alt="Bounded coordinate memory structure" width="600">

### Figure 4. Priority reinforcement and local eviction dynamics

<img src="figures/Figure_4_Priority_Reinforcement_and_Local_Eviction_Dynamics.png" alt="Priority reinforcement and local eviction dynamics" width="700">
