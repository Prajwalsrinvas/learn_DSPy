# DSPy: Build & Optimize Agentic Apps 🤖⚡

- Code files from the deeplearning.ai [short course on DSPy: Build & Optimize Agentic Apps](https://www.deeplearning.ai/short-courses/dspy-build-optimize-agentic-apps/)
- [Certificate](https://learn.deeplearning.ai/accomplishments/040d4219-1cca-4b4b-8419-b9cc08c43298?usp=sharing)

## Why DSPy? 🧩

DSPy transforms how we build AI applications by shifting from fragile prompt engineering to robust programming paradigms:

- **Programming, not prompting** - Write modular AI software with structured code instead of brittle strings
- **Automatic optimization** - Compile AI programs into effective prompts and weights using built-in optimizers
- **Model agnostic** - Build once, deploy across different language models and inference strategies
- **Faster iteration** - Focus on system design rather than prompt tweaking and manual tuning
- **Reliability** - Reduce hallucinations and improve consistency through structured approaches
- **Composability** - Build complex agent systems by combining simple, reusable modules

## Core DSPy Concepts 🛠️

### 1. Signatures
Define input/output behavior as natural language specifications that guide model behavior.
```python
# Simple signature
"question -> answer"

# Typed signature with field descriptions
"question: str -> reasoning: str, answer: float"
```

### 2. Modules
Assign strategies for invoking language models with different reasoning approaches.
```python
# Basic prediction
dspy.Predict("question -> answer")

# Chain of thought reasoning
dspy.ChainOfThought("question -> answer")

# ReAct agent with tools
dspy.ReAct("question -> answer", tools=[search_tool])
```

### 3. Optimizers
Automatically tune prompts and weights to improve performance on your specific tasks.
```python
# Bootstrap few-shot examples
dspy.BootstrapRS(metric=my_metric)

# Optimize instructions and examples
dspy.MIPROv2(metric=my_metric, auto="light")

# Fine-tune model weights
dspy.BootstrapFinetune(metric=my_metric)
```

| No. | Concepts | NBSanity | GitHub |
|-----|----------|----------|--------|
| 1 | • Introduction to DSPy signatures<br>• Building modular AI components<br>• Predict vs ChainOfThought modules<br>• Defining input/output behavior<br>| [![Open In NBSanity](https://nbsanity.com/assets/icon.png)](https://nbsanity.com/Prajwalsrinvas/learn_DSPy/blob/main/1_modules_and_signatures.ipynb) | [![GitHub](https://cdn-icons-png.flaticon.com/32/270/270798.png)](https://github.com/Prajwalsrinvas/learn_DSPy/blob/main/1_modules_and_signatures.ipynb) |
| 2 | • Building DSPy agents with tools<br>• MLflow integration for tracing<br>• Visualizing agent execution flows | [![Open In NBSanity](https://nbsanity.com/assets/icon.png)](https://nbsanity.com/Prajwalsrinvas/learn_DSPy/blob/main/2_agent_with_mlflow_tracing.ipynb) | [![GitHub](https://cdn-icons-png.flaticon.com/32/270/270798.png)](https://github.com/Prajwalsrinvas/learn_DSPy/blob/main/2_agent_with_mlflow_tracing.ipynb) |
| 3 | • Automatic prompt optimization<br>• DSPy optimizers (MIPROv2, BootstrapRS)<br>• Metrics and evaluation strategies<br>| [![Open In NBSanity](https://nbsanity.com/assets/icon.png)](https://nbsanity.com/Prajwalsrinvas/learn_DSPy/blob/main/3_dspy_optimizer.ipynb) | [![GitHub](https://cdn-icons-png.flaticon.com/32/270/270798.png)](https://github.com/Prajwalsrinvas/learn_DSPy/blob/main/3_dspy_optimizer.ipynb) |

## Resources 📚

- [DSPy Learning Hub](https://dspy.ai/learn/)
- [DSPy Tutorials](https://dspy.ai/tutorials/)
- [DSPy GitHub Repository](https://github.com/stanfordnlp/dspy)
- [DSPy Documentation](https://dspy.ai/)
- [MLflow Documentation](https://mlflow.org/docs/latest/index.html)