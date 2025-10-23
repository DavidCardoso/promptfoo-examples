# getting-started

This is a simple example that demonstrates the basic functionality of promptfoo. It tests two different translation prompts across multiple language models.

You can create this example with:

```bash
npx promptfoo@latest init --example getting-started
```

## Setup

1. Set your API keys:

```shell
export LITELLM_API_KEY=your-key-here
# export others according to the LLM used
```

2. Run the evaluation:

```bash
promptfoo eval
```

## What's happening?

This example:

- Tests two different ways to phrase a translation prompt
- Compares outputs between different models
- Uses two test cases with different languages and inputs

The configuration in `promptfooconfig.yaml` shows:

- How to define prompts with variables using `{{variable_name}}`
- How to specify multiple providers (models)
- How to set up test cases with different variable values

This is the same example shown in the Getting Started guide at https://promptfoo.dev/docs/getting-started
