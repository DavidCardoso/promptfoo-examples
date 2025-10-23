# self-grading

This example shows how you can have an LLM grade its own output according to predefined expectations.

You can create this example with:

```shell
npx promptfoo@latest init --example self-grading
```

## Setup

1. Set your API keys:

```shell
export LITELLM_API_KEY=your-key-here
export GITHUB_TOKEN=your-key-here
# export others according to the LLM used
```

2. Run the evaluation:

```shell
promptfoo eval
```

You can also define the tests in a CSV file:

```shell
promptfoo eval --tests tests.csv
```

## What's happening?

This example:

- Tests two different prompt styles for an e-commerce chatbot
- Evaluates responses using custom scoring criteria
- Compares outputs between different LLM models
- Uses multiple test cases with varied customer scenarios

The configuration in `promptfooconfig.yaml` shows:

- How to define prompts with variables using `{{name}}` and `{{question}}`
- How to specify multiple LLM providers via LiteLLM
- How to set up custom JavaScript-based assertions for response evaluation
- How to configure default test options for all test cases
- How to structure test cases for different customer service scenarios

Key features demonstrated:

1. **Custom Assertions**: Uses a JavaScript function to score responses based on length (shorter is better)
2. **Multiple Test Cases**: Tests 10 different customer service scenarios
3. **Prompt Variations**: Tests two different prompt styles:
   - Formal e-commerce chat assistant
   - Bubbly customer service representative
4. **Default Test Options**: Shows how to configure provider options that apply to all tests
5. **File Organization**: Demonstrates a structured approach with separate directories for prompts, tests, and data

This example showcases Promptfoo's advanced evaluation capabilities beyond simple string matching, allowing for sophisticated response quality assessment.
