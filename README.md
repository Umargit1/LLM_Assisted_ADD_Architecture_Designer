# LLM Assisted ADD Architecture Designer

This repository contains an experimental Google Colab implementation of **LLM assisted software architecture design** based on the **Attribute Driven Design (ADD)** methodology.

The project explores how large language models can support structured architectural reasoning when guided by an explicit design process, clearly defined roles, and iterative architectural artifacts.

---

## Motivation

Large language models are increasingly used to assist with software design tasks. However, when used with unstructured prompting, their outputs are often inconsistent, difficult to reproduce, and weak in architectural reasoning.

This project is motivated by the idea that:

- A **formal architecture design process** can provide necessary structure
- Explicit step by step guidance improves consistency
- The **reasoning capability of the underlying LLM** remains a critical factor in design quality

The notebook is intended as a research and experimentation tool rather than a fully automated architecture generator.

---

## What This Notebook Does

The notebook implements a structured ADD based workflow that includes:

- Explicit encoding of ADD steps as prompts
- A centralized architecture document that evolves across iterations
- Iterative reasoning driven by prioritized quality attributes
- Generation of architectural views using Mermaid syntax
- Comparative evaluation of different LLMs under the same design constraints

The workflow assumes a **collaborative design setting**, where the human architect actively reviews, refines, and validates each step.

---

## Models Evaluated

The notebook has been evaluated using multiple large language models, including:

- Llama 3.3 70B (via Groq)
- OpenAI GPT 4o

Clear differences were observed in the ability of these models to:

- Follow multi step architectural reasoning
- Maintain architectural context across iterations
- Produce consistent and syntactically valid architectural diagrams

These results highlight the importance of strong instruction following and reasoning capabilities for effective LLM assisted architecture design.

---

## Key Observations

Some recurring observations from the experiments include:

- The ADD process provides important structural guidance but does not fully compensate for weaker reasoning models
- Lower capability models require significant human oversight to correct hallucinations and syntax errors
- Diagram correctness can serve as a practical signal of architectural coherence
- Architectural design remains most effective as a collaboration between the human architect and the LLM

---

## How to Use

1. Open the notebook in Google Colab
2. Provide a system description and prioritized quality attributes
3. Execute the ADD workflow step by step
4. Review and refine architectural outputs after each iteration
5. Optionally compare results across different LLMs

The notebook is designed for **interactive use**, with human judgment playing a central role.

---

## Limitations

- Results depend heavily on the selected LLM
- Human review is required at every stage
- The focus is on early stage architectural design rather than detailed implementation

---

## Future Work

Potential extensions include:

- Explicit iteration planning and documentation
- Logging of architectural decisions and tradeoffs
- Evaluation across a broader range of LLMs
- Integration with formal architecture documentation tools

---

## License

This project is shared for research and educational purposes.
