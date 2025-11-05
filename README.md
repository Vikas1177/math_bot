# Math Problem Solver Agent

This project is an intelligent AI agent that solves math problems by decomposing complex problems into sub-problems, generating and executing Python code, and leveraging large language models (LLMs) for explanations and calculations.

---

## Features
- Classifies math problems based on complexity (simple or complex).
- Decomposes complex problems into manageable sub-problems with clear mathematical tasks.
- Generates safe and optimized Python code to solve sub-problems.
- Uses fallback mechanisms with LLMs to handle unsolvable or difficult problems.
- Executes generated code securely with strict import and unsafe code checks.
- Maintains context and solution state throughout the multi-step solving workflow.
- Provides concise, direct answers without unnecessary explanations.

---

## Architecture
- Workflow graph managing states such as classification, decomposition, code generation, execution, fallback, and LLM solving.
- Typed dictionaries for problem states, contexts, and solutions.
- Integration with LangChain and Google Generative AI for LLM interactions.
- Error handling and safe execution environments for generated code.

---

## Usage
1. Define a math problem with initial conditions or parameters.  
2. The agent classifies problem complexity.  
3. Complex problems are broken down; code is generated and executed step-by-step.  
4. If code execution fails, the LLM fallback solver attempts the problem.  
5. Final concise solutions are returned with step-wise explanations if needed.

---

## Requirements
- Python 3.10+
- Libraries: `LangChain`, `Google Generative AI SDK`, `numpy`, `sympy`, `scipy`, `IPython`
- API keys for `LangSmith` and `Google Gemini AI` as environment variables

---

---

## Contribution
Contributions are welcome for improving problem classification, code generation heuristics, and adding support for more mathematical domains.
