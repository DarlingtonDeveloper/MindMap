**System, Contextual, and Role Prompting** are identified as key **prompting techniques** used to guide how Large Language Models (LLMs) generate text. These techniques are crucial within the larger context of **Prompt Engineering**, which is the process of crafting effective prompts to obtain meaningful output from LLMs. The sources emphasize that prompt engineering is an **iterative process** where various aspects of a prompt, such as word choice, style, tone, structure, and context, can affect the model's efficacy.

**System Prompting**

- **Sets the overall context and purpose** for the language model. It defines the 'big picture' of what the model should be doing, such as translating a language or classifying a review. The source explicitly states that the name ‘system prompt’ actually stands for ‘**providing an additional task to the system**’.
- **Defines the model’s fundamental capabilities and overarching purpose**.
- **Can be useful for generating output that meets specific requirements**. Examples include generating code snippets compatible with a specific programming language or returning output in a certain structure, such as JSON format. Table 3 in the source provides an example where a system prompt is used to classify movie reviews and specifies that only the uppercase label should be returned.
- **Can be really useful for safety and toxicity**. Adding a line like ‘You should be respectful in your answer’ to a system prompt can help control the output.
- Table 3 illustrates a system prompt example where the goal is to classify movie reviews, and the prompt includes the instruction to only return the label in uppercase. The model used is `gemini-pro` with specific temperature and token limits set, though the clear instruction ensured no extra text was returned.

**Contextual Prompting**

- **Provides specific details or background information relevant to the current conversation or task**. It helps the model understand the nuances of what’s being asked and tailor the response accordingly.
- Provides **immediate, task-specific information** to guide the response. It is **highly specific to the current task or input**, which is dynamic.
- Table 7 in the source shows an example of contextual prompting.

**Role Prompting**

- **Assigns a specific character or identity for the language model to adopt**. This helps the model generate responses that are consistent with the assigned role and its associated knowledge and behavior. Examples provided include role-playing as a book editor, a kindergarten teacher, or a motivational speaker.
- Frames the model’s **output style and voice**, adding a layer of specificity and personality. Table 5 shows an example where the model takes on the role of a travel guide. You can also specify styles such as humorous or inspirational. Table 6 provides an example of a prompt instructing the model to act as a humorous travel guide.
- Defining a role perspective gives the AI model a **blueprint of the tone, style, and focused expertise** to improve the quality, relevance, and effectiveness of the output.

**Relationship and Overlap**

The sources highlight that there can be **considerable overlap** between system, contextual, and role prompting. For instance, a prompt that assigns a role to the system can also include contextual information.

However, each technique has a **slightly different primary purpose**:

- **System prompt:** Defines the model’s fundamental capabilities and overarching purpose.
- **Contextual prompt:** Provides immediate, task-specific information to guide the response and is dynamic to the current input.
- **Role prompt:** Frames the model’s output style and voice, adding specificity and personality.

Distinguishing between these types of prompts provides a **framework for designing prompts with clear intent**, allowing for **flexible combinations** and making it easier to analyze how each prompt type influences the language model’s output. These techniques are fundamental tools within the broader field of prompt engineering, enabling practitioners to elicit more controlled and relevant responses from LLMs. The clearer the prompt text, the better the LLM can predict the next likely text.