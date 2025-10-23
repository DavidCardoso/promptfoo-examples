# Promptfoo Examples

A collection of examples demonstrating how to use Promptfoo for LLM prompt testing and evaluation.

- [Promptfoo Examples](#promptfoo-examples)
  - [Repository Structure](#repository-structure)
  - [What is Promptfoo?](#what-is-promptfoo)
  - [CLI Commands Quick Reference](#cli-commands-quick-reference)
  - [Examples](#examples)
    - [Getting Started](#getting-started)
    - [Self-Grading](#self-grading)
  - [References](#references)

## Repository Structure

```
promptfoo-examples/
├── getting-started/     # Basic examples to get started with Promptfoo
└── self-grading/       # Examples of self-grading prompts evaluation
```

## What is Promptfoo?

Promptfoo is a powerful command-line tool designed for testing and evaluating LLM (Large Language Model) prompts. It helps developers and prompt engineers to:

- Test prompts across multiple LLM providers (OpenAI, Anthropic, etc.)
- Evaluate prompt variations against test cases
- Automate prompt testing with assertion-based validation
- Generate detailed evaluation reports
- Compare different model outputs side-by-side
- Track prompt performance over time

## CLI Commands Quick Reference

Here are some essential Promptfoo commands used in this repository:

```bash
# Initialize a new Promptfoo project
promptfoo init

# Run evaluations defined in promptfooconfig.yaml
promptfoo eval

# Generate a shareable HTML report
promptfoo eval --output-format html --output report.html

# View tests in the browser
promptfoo view
```

## Examples

### Getting Started
Located in `/getting-started/`

This example demonstrates the basic setup and usage of Promptfoo, including:
- Basic configuration with `promptfooconfig.yaml`
- Setting up providers (LLM models)
- Writing simple prompt variations
- Creating basic test assertions
- Working with environment variables

[Go to Getting Started Example →](./getting-started/)

### Self-Grading
Located in `/self-grading/`

This example shows how to implement self-grading evaluations, featuring:
- Advanced assertion configurations
- Custom grading criteria
- Model-based evaluation strategies
- Output validation techniques

[Go to Self-Grading Example →](./self-grading/)

## References

For more detailed information, refer to the official Promptfoo documentation:

- [Configuration Guide](https://promptfoo.dev/docs/configuration/guide) - Learn about `promptfooconfig.yaml` options
- [Providers](https://promptfoo.dev/docs/providers) - Supported LLM providers and setup
- [Writing Tests](https://www.promptfoo.dev/docs/configuration/expected-outputs/#using-assertions) - Test case creation and assertions
- [Command Line Usage](https://www.promptfoo.dev/docs/usage/command-line/) - Complete CLI reference
- [Environment Variables](https://www.promptfoo.dev/docs/usage/command-line/) - Working with environment variables
- [Output Formats](https://promptfoo.dev/docs/configuration/outputs) - Available output formats and reporting
- [Self-hosting Promptfoo server](https://www.promptfoo.dev/docs/usage/self-hosting/) - Check how to self-host it for local development and testing
- [Model-graded metrics](https://www.promptfoo.dev/docs/configuration/expected-outputs/model-graded/) - Grading strategies