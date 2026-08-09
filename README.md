# AI Factual Accuracy & Uncertainty Control Framework

This project provides an experimental, user-level instruction set designed to influence how an AI model handles incomplete information, distinguishes between types of evidence, and manages uncertainty.

It does **not** add knowledge, retrain, or modify the underlying model. Instead, it provides a structured prompt framework to enforce rigorous evidence handling.

## Purpose
This framework was developed to address common AI behaviors where models sound convincing despite relying on unsupported inferences, outdated information, or a mix of factual and calculated values. It is particularly effective for:
- Technical specifications
- Performance measurements
- Historical dates
- Scientific claims
- Managing conflicting sources

## How to use
Copy the contents of `RULES.md` into your system prompt or custom instructions (e.g., in a Custom GPT, System Message, or AI assistant configuration).

## License
This project is licensed under the MIT License. See the LICENSE file for details.
