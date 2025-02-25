# LLM Prompt Collection

A comprehensive repository for organizing, documenting, and sharing effective prompts for Large Language Models (LLMs) such as GPT-4, Claude, Llama, and others.

## Purpose

This repository serves as a personal knowledge base for:
- Storing successful prompts that produce great results
- Documenting prompt engineering techniques
- Tracking the evolution of prompts across different projects
- Sharing prompt templates that can be reused and adapted

## Repository Structure

```
llm-prompt-collection/
├── categories/                 # Prompts organized by category
│   ├── coding/                 # Prompts related to programming tasks
│   ├── writing/                # Prompts for content creation
│   ├── data-analysis/          # Prompts for data processing and analysis
│   └── creative/               # Prompts for creative tasks
├── models/                     # Prompts organized by LLM
│   ├── gpt-4/                  # GPT-4 specific prompts
│   ├── claude/                 # Claude specific prompts
│   └── other-models/           # Prompts for other LLMs
├── templates/                  # Reusable prompt templates
├── examples/                   # Complete examples with prompt and response
└── resources/                  # Useful resources about prompt engineering
```

## How to Use This Repository

### Adding a New Prompt

1. Determine the appropriate category for your prompt
2. Create a new markdown file or add to an existing one
3. Follow the prompt template format (see below)
4. Include relevant metadata and examples

### Prompt Template Format

Each prompt should be documented using this format:

```markdown
# [Prompt Title]

## Metadata
- **Created**: YYYY-MM-DD
- **Model**: [Model used, e.g., GPT-4, Claude 3.5, etc.]
- **Category**: [e.g., Coding, Writing, Data Analysis]
- **Tags**: [comma-separated list of relevant tags]

## Prompt
\`\`\`
[The actual prompt text goes here]
\`\`\`

## Purpose
[Brief description of what this prompt aims to achieve]

## Example Usage
[Example of how to use this prompt, possibly with variables to replace]

## Sample Response
[Optional: Include a sample response from the LLM]

## Notes
[Any additional notes, variations, or improvements]
```

## Best Practices

- **Be specific**: Clearly define what you want the LLM to do
- **Provide context**: Give necessary background information
- **Use examples**: Include examples when possible to guide the model
- **Document constraints**: Note any limitations or requirements
- **Version your prompts**: Track changes and improvements over time

## Contributing

This is a personal repository, but if you're collaborating with me:
1. Fork the repository
2. Create a new branch for your changes
3. Submit a pull request with a clear description

## License

This repository is for personal use. All rights reserved.