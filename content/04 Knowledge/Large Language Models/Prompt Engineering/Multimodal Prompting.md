Multimodal prompting** is a significant area within the broader context of **prompt engineering**, representing an evolution beyond traditional text-based interactions with Large Language Models (LLMs).

Here's a breakdown of what the sources say:

- **Definition:** Multimodal prompting is a technique where you use **multiple input formats** such as text, images, audio, code, or other modalities, in conjunction, to guide an LLM, rather than relying solely on text prompts. This allows for richer and more versatile ways to interact with and instruct these models.
    
- **Emerging Capability:** The sources highlight that **multimodality is a major axis along which LLMs are rapidly improving**. This indicates that it's a key direction in the development of more advanced and capable language models.
    
- **Examples of Multimodal Capabilities:** The sources provide several examples of how multimodality manifests in LLMs:
    
    - **Image Generation:** LLMs can generate images based on text prompts. While the current implementation (like with DALL-E 3 in some cases) might involve a separate image generation model receiving a text caption from the LLM, it still represents a form of multimodal output driven by a text prompt.
    - **Image Understanding:** LLMs are gaining the ability to "see" images provided as input and process that visual information to perform tasks, such as writing code based on a sketched website diagram.
    - **Audio Processing:** Some LLMs can now "hear" and "speak," enabling speech-to-speech communication, moving beyond text-only interactions.
    - **Video Understanding:** Advanced features allow models to "see" a video feed and respond based on the visual content presented.
- **Underlying Mechanism: Tokenization:** The ability to handle diverse modalities often relies on the principle of **tokenization**. Just as text is broken down into tokens, audio (e.g., spectrogram slices) and images (e.g., patches) can also be tokenized and represented as sequences. This allows the same underlying language models to process and understand these different forms of input by treating them as sequences of tokens within their context window.
    
- **Distinction from Code Prompting:** While code can be one of the modalities used in multimodal prompting, the sources clarify that **prompting for code is generally considered a separate concern**. Code prompting, as discussed earlier, uses regular LLMs and text prompts specifically for code-related tasks like writing, explaining, translating, and debugging code. Multimodal prompting extends beyond code to include other non-textual input formats.
    
- **Future Implications:** The development of native multimodal capabilities within LLMs promises to **enable more natural and intuitive conversations** and interactions. It moves towards a more holistic understanding of the world, where models can process and reason across different types of information simultaneously.
    

In summary, multimodal prompting is an expanding frontier in prompt engineering that leverages the increasing ability of LLMs to process and generate information across various modalities beyond just text. By using combinations of different input types, prompt engineers can unlock new possibilities for interacting with and harnessing the power of these advanced AI models.