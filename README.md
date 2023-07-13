# LLM Workflow Engine (LWE) Zap plugin

Zap plugin for [LLM Workflow Engine](https://github.com/llm-workflow-engine/llm-workflow-engine)

Send natural language commands to Zapier actions: https://nla.zapier.com/get-started/

## Installation

### From packages

Install the latest version of this software directly from github with pip:

```bash
pip install git+https://github.com/llm-workflow-engine/lwe-plugin-zap
```

### From source (recommended for development)

Install the latest version of this software directly from git:

```bash
git clone https://github.com/llm-workflow-engine/lwe-plugin-zap.git
```

Install the development package:

```bash
cd llm-workflow-engine
pip install -e .
```

## Configuration

Add the following to `config.yaml` in your profile:

```yaml
plugins:
  enabled:
    - zap
    # Any other plugins you want enabled...
  # These are the default values.
  zap:
    agent:
      verbose: true
```

## Usage

From a running LWE shell:

```
/zap send an email to foo@bar.com with a random top 10 list
```
