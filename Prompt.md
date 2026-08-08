# Prompt Engineering Fundamentals

## 1. Core Definitions

- **Prompt:** A piece of text, instruction, or query used to prompt and guide a Large Language Model (LLM) to produce a specific response.
- **Prompt Engineering:** The practice of structuring, refining, and crafting clear instructions to guide AI systems toward optimal outputs.

### LLM Characteristics
- **Volume of Training Data:** Trained on extensive datasets spanning web, literature, and code.
- **Contextual Understanding:** Comprehends semantic nuances across long inputs.
- **Machine Learning Integration:** Employs probabilistic token prediction and fine-tuning.
- **Versatility:** Capable of handling diverse tasks (writing, coding, summarizing, reasoning).

---

## 2. Model Tuning Methods

| Method | Description |
| :--- | :--- |
| **Fine-Tuning** | Adjusts all or most parameters of a pre-trained model on custom datasets for domain specialization. |
| **LoRA** *(Low-Rank Adaptation)* | A parameter-efficient fine-tuning technique that freezes original model weights and injects trainable rank decomposition matrices. |

---

## 3. AI Output Formatting

- **Raw Text:** Unformatted, raw textual responses.
- **Structured Text:** Text organized using Markdown elements (headings, bullet points, numbered lists, blockquotes, delimiters).
- **Formatted Data:** Machine-readable output formats such as `JSON`, `YAML`, `XML`, or `HTML`.

---

## 4. Prompt Parameters

### Basic Parameters
- **Temperature:** Controls randomness and creativity ($0.0$ for deterministic/strict, $1.0$ for highly creative).
- **Max Tokens:** Sets the upper limit on the total tokens generated in the response.

### Advanced Parameters
- **Sampling Parameters:** Controls token selection probability distribution (e.g., Top-P / Nucleus Sampling, Top-K).
- **Stop Sequences:** Specified characters, phrases, or symbols that signal the model to cease generation immediately.

---

## 5. Prompting Techniques

### 🎯 Shot-Based Prompting
Refers to the number of demonstration examples provided within the prompt context:
- **Zero-Shot Prompting:** Requesting a task without providing any demonstration examples.
- **Few-Shot Prompting:** Providing a few input-output examples in the prompt to demonstrate the target format and behavior.

### 🔗 Sequential Prompting
- **Chain-of-Thought (CoT):** Encourages the model to break down complex reasoning into explicit, step-by-step intermediate thoughts before providing the final answer.
- **Prompt Chaining:** Breaking a complex task into a series of smaller, interconnected prompts where the output of one step feeds into the next.

### 🧭 Context-Guiding Techniques
- **Hinting:** Nudging the model by introducing specific keywords or concept hints.
- **Directional Stimulus Prompting (DSP):** Providing explicit directional hints or key phrase stimuli to guide model generation.
- **Generated Knowledge Prompting (GKP):** Asking the LLM to generate relevant background knowledge first before answering the final question.

---

## 6. Prompting Best Practices

### Writing Effective Prompts
1. **Clear & Specific Requests:** Clearly specify the desired action, target audience, format, and tone.
2. **Maintain Focus:** Avoid irrelevant context or contradictory instructions.
3. **Manage Input Length:** Keep context concise and within effective model bounds.
4. **Use Visual Delimiters:** Structure input using tags, markdown headers, or triple quotes (`"""`).
5. **Fresh Dialogues:** Start a new chat context when switching to unrelated tasks.

### Refining Prompts
- 🔄 **Regenerate Results:** Test multiple generations to observe variance.
- ✏️ **Rephrase Prompt:** Clarify ambiguous phrasing or reorganize instructions.
- ⚙️ **Adjust Parameters:** Fine-tune temperature or sampling parameters.
- 🧩 **Apply Advanced Techniques:** Introduce Chain-of-Thought or Few-Shot examples.
- 🔪 **Decompose Complex Tasks:** Break large objectives into sequential sub-prompts.



