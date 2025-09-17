# Test170925 Crew

Welcome to the Test170925 Crew project, powered by [crewAI](https://crewai.com). This template is designed to help you set up a multi-agent AI system with ease, leveraging the powerful and flexible framework provided by crewAI. Our goal is to enable your agents to collaborate effectively on complex tasks, maximizing their collective intelligence and capabilities.

## Installation

Ensure you have Python >=3.10 <3.14 installed on your system.

### Quick start (macOS & Linux)

```bash
# Create and activate a virtual environment
python3 -m venv .venv
source .venv/bin/activate

# Install the project dependencies
pip install -r requirements.txt

# Prepare your environment variables
cp .env.example .env
open .env  # fill in your provider API keys
```

Once the `.env` file is configured you can immediately run the crew locally with `crewai run` (see [Running the Project](#running-the-project)).

### Using uv (optional)

This project is also compatible with [UV](https://docs.astral.sh/uv/) for dependency management:

```bash
pip install uv
uv sync
```
### Customizing

**Copy `.env.example` to `.env` and add your provider keys (e.g. `OPENAI_API_KEY`)**

- Modify `src/test_170925/config/agents.yaml` to define your agents
- Modify `src/test_170925/config/tasks.yaml` to define your tasks
- Modify `src/test_170925/crew.py` to add your own logic, tools and specific args
- Modify `src/test_170925/main.py` to add custom inputs for your agents and tasks

## Running the Project

To kickstart your crew of AI agents and begin task execution, run this from the root folder of your project:

```bash
$ crewai run
```

This command initializes the test_170925 Crew, assembling the agents and assigning them tasks as defined in your configuration.

This example, unmodified, will run the create a `report.md` file with the output of a research on LLMs in the root folder.

## Understanding Your Crew

The test_170925 Crew is composed of multiple AI agents, each with unique roles, goals, and tools. These agents collaborate on a series of tasks, defined in `config/tasks.yaml`, leveraging their collective skills to achieve complex objectives. The `config/agents.yaml` file outlines the capabilities and configurations of each agent in your crew.

## Support

For support, questions, or feedback regarding the Test170925 Crew or crewAI.
- Visit our [documentation](https://docs.crewai.com)
- Reach out to us through our [GitHub repository](https://github.com/joaomdmoura/crewai)
- [Join our Discord](https://discord.com/invite/X4JWnZnxPb)
- [Chat with our docs](https://chatg.pt/DWjSBZn)

Let's create wonders together with the power and simplicity of crewAI.
