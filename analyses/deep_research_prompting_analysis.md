### 1. Executive Summary

- 1 new primary framework identified: Deep Research Prompting (DRP).
- Adds capabilities for structural archetyping (Typological Stack, Lens-Driven Analysis) and complex iteration (ReAct, Recursive Criticism).
- Expected impact: "foundational" for moving standard prompt workflows into research-grade, strategist-level pipelines.

### 2. Document-Level Framework Extraction

#### 2.1 PromptResearch/Deep Research Prompt Engineering_.md

- **Framework Name**: Deep Research Prompting (DRP)
- **Core Innovation**: Moving beyond basic queries to designing prompts as instruments of epistemic control, structuring the analytical and cognitive workflow.
- **Key Components / Sub-Modules**: Typological Stack, Lens-Driven Analysis, Constraint-Directed Inquiry, Counterfactual Exploration, CoT, ReAct, Recursive Criticism.
- **Complexity Level**: Advanced
- **Primary Contribution**: Provides a taxonomy of advanced prompting patterns aimed at eliciting insight generation rather than mere summarization.
- **Intended Use Cases**: Complex research, strategic analysis, insight generation, policy analysis.
- **Prerequisites / Dependencies**: Large LLMs capable of multi-step reasoning.

### 3. Normalized Framework Catalog

- **Name**: Deep Research Prompting (DRP)
- **Type**: Orchestration pattern / Cognitive scaffolding
- **Core Mechanisms**:
  - Typological Stacking (multi-persona simulation)
  - Lens-Driven Analysis (theoretical application)
  - Explicit Constraints
  - CoT / ReAct / RCI loops
- **Input / Output Contract**: Expects high-level research questions; produces structured, multi-dimensional analysis and insights.
- **Typical Integration Point in PEW**: Prompt design and multi-agent orchestration.
- **Complexity Tier**: Advanced

### 4. Integration Mapping to Existing Workbench

#### 4.1 Extensions of Existing Frameworks

- **PALS Extension**: Enhances the Cognitive and Trust & Epistemics layers by providing concrete structural patterns (e.g., Typological Stacks) for directing attention and reasoning.
- **Context Engineering 2.0**: The DRP constraints map directly onto the CxEP post-conditions and invariants.
- **Role Prompting**: Directly extends Role Prompting with the "Typological Stack" pattern (simulating multiple interacting functions within a persona).

#### 4.2 New Modules and Services

- **New Services**: "Typological Stack Composer", "Lens-Driven Analysis Router"
- **Data Models**: New fields in the PRP schema to define "Analytical Lens" and "Counterfactual Variables".
- **Workflow Slots**: During the initial prompt design phase and within ReAct/RCI loops in the execution engine.

### 5. Proposed Workbench Architecture Updates

- **Core Engine Changes**: Add native support for ReAct and Recursive Criticism (RCI) loops within the execution engine.
- **Integration Layer**: Create a "Lens Application Engine" that maps specific theoretical frameworks to incoming prompts.
- **User Interface Additions**: Add a "Typological Stack Builder" to the Role Prompting workspace and a "Lens Selector" to the prompt builder.
- **Advanced Workflow Engine**: Support for recursive prompt execution (RCI loops).

### 6. Implementation Roadmap

- **Phase 1: Foundation (0–2 months)**
  - **Goals**: Implement basic Constraint-Directed Inquiry and Typological Stack patterns.
  - **Deliverables**: Typological Stack Builder UI, constraint validation in CxEP.
  - **Technical Risks**: Prompt length limits with complex typological stacks.
  - **Dependencies**: Existing PALS and Role Prompting workspaces.

- **Phase 2: Intermediate (2–6 months)**
  - **Goals**: Deploy the Lens-Driven Analysis routing and basic CoT scaffolding.
  - **Deliverables**: Lens Selector UI, pre-built lens library, automated CoT injection.
  - **Technical Risks**: Lens abstraction might be too vague for certain models.
  - **Dependencies**: Phase 1 completion.

- **Phase 3: Advanced (6–12+ months)**
  - **Goals**: Implement full ReAct and RCI (Recursive Criticism and Improvement) loops.
  - **Deliverables**: Recursive execution engine, ReAct tool integration, automated self-refinement pipelines.
  - **Technical Risks**: Infinite loops in recursive prompting, high API costs.
  - **Dependencies**: Advanced Workflow Engine overhaul.

### 7. Success Metrics and Evaluation

- **Quantitative Metrics**:
  - Prompt quality improvements: Increase in "Insight Generation" scores vs. "Summarization" scores on a standardized test set.
  - RCI loop efficiency: Number of iterations to reach passing state.
- **Qualitative Metrics**:
  - Researcher satisfaction with Lens-Driven Analysis outputs.
  - Novel insights generated via Counterfactual Exploration patterns.

### 8. Research-to-Practice Translation

- **Recommended Starter Workflows**: Start with the Typological Stack Builder to define complex personas, then apply a specific Analytical Lens to a dataset.
- **Suggested Personas**: Researchers (using Lens-Driven Analysis), Strategists (using Counterfactual Exploration).
- **Collaboration**: Open repository of Analytical Lenses and Typological Stack templates.
