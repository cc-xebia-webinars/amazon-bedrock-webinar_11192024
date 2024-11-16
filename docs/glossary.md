# Glossary

- **logic** - In the context of machine learning, particularly in classification tasks and neural networks, a **logit** is the raw, unnormalized output of a model's prediction before applying an activation function like softmax or sigmoid. 

    For example, in a neural network used for classification, the final layer might output a vector of logits, where each element corresponds to a class. These logits are then transformed into probabilities using an activation function:

    - **Softmax**: Converts logits into probabilities that sum to 1, typically used for multi-class classification.
    - **Sigmoid**: Converts logits into probabilities between 0 and 1, typically used for binary classification.

    Logits can be thought of as scores that indicate the relative likelihood of each class before normalization.

- **nucleus sampling** - Nucleus sampling, also known as top-p sampling, is a technique used in natural language processing for generating text. It is designed to balance the trade-off between diversity and coherence in the generated text.

    Here's how it works:
    1. **Probability Distribution**: The model generates a probability distribution over the possible next tokens.
    2. **Sorting**: The tokens are sorted based on their probabilities in descending order.
    3. **Cumulative Probability**: The cumulative probability of the sorted tokens is calculated.
    4. **Threshold**: A threshold `p` (e.g., 0.5) is set. The smallest set of tokens whose cumulative probability is at least `p` is selected.
    5. **Sampling**: The next token is sampled from this set of tokens.

    By using nucleus sampling, the model considers only the most probable tokens up to the cumulative probability threshold, which helps in generating more coherent and contextually relevant text while still allowing for some diversity.

- **prompt engineering** - Prompt engineering is the process of designing and refining input prompts to effectively interact with and elicit desired responses from large language models (LLMs) like GPT-4. It involves crafting the input text in a way that guides the model to generate relevant, accurate, and contextually appropriate outputs.

    Key aspects of prompt engineering include:

    1. **Clarity:** Ensuring the prompt is clear and unambiguous.
    1. **Context:** Providing sufficient context to guide the model's response.
    1. **Specificity:** Being specific about the desired output to reduce variability.
    1. **Iterative Refinement:** Continuously refining the prompt based on the model's responses to improve the quality of the output.
    
    Prompt engineering is crucial for applications such as chatbots, automated content generation, and other AI-driven tasks where precise and relevant outputs are essential.

- Retreival Augmented Generation (RAG) - A framework that combines the strengths of retrieval-based and generation-based models in natural language processing tasks. RAG models leverage a pre-trained retriever to fetch relevant information from a large corpus and then use a generative model to generate responses based on the retrieved information.

    Key components of RAG include:
    1. **Retriever**: A pre-trained model that efficiently retrieves relevant passages or documents from a large corpus based on the input query or context.
    2. **Generator**: A generative model, such as GPT-3 or GPT-4, that takes the retrieved information as input and generates coherent and contextually relevant responses.
    3. **Ranker**: An optional component that ranks the retrieved passages to select the most relevant ones for input to the generator.

    RAG models are effective in tasks that require a combination of factual accuracy, context awareness, and creative generation, such as question answering, dialogue systems, and content creation. By integrating retrieval and generation components, RAG models achieve a balance between factual accuracy and fluency in generated text.

- **ReAct pattern** - A framework used in working with large language models (LLMs) and AI to improve their interaction and decision-making capabilities. It stands for **Reasoning and Acting** and involves a structured approach to guide the model through a sequence of reasoning steps and actions to achieve a desired outcome.

    Key components of the ReAct pattern include:
    1. **Reasoning**: The model is prompted to think through a problem or scenario step-by-step, breaking it down into smaller, manageable parts. This helps in understanding the context and formulating a coherent plan.
    2. **Acting**: Based on the reasoning, the model takes specific actions or generates responses that are aligned with the goals of the task.

    The ReAct pattern is particularly useful in complex tasks where the model needs to perform multiple steps or make decisions based on intermediate results. It helps in improving the accuracy, relevance, and coherence of the model's outputs.

    Applications of the ReAct pattern include:
    - **Task Automation**: Automating multi-step processes where each step depends on the outcome of the previous one.
    - **Interactive Systems**: Building chatbots and virtual assistants that can handle complex queries by reasoning through them.
    - **Problem Solving**: Enhancing the model's ability to solve problems that require logical reasoning and sequential actions.

- Zero-shot ReAct - A variant of the ReAct pattern that involves guiding large language models (LLMs) through a sequence of reasoning and acting steps without providing any training examples or labeled data. In zero-shot ReAct, the model is expected to perform a task or generate responses based on a prompt or input without any explicit supervision.

    Key features of zero-shot ReAct include:
    1. **Prompt-based Guidance**: The model receives a prompt or input that outlines the task or scenario it needs to reason through and act upon.
    2. **Reasoning Steps**: The model goes through a series of reasoning steps to understand the context, constraints, and goals of the task.
    3. **Action Generation**: Based on the reasoning, the model generates responses or takes actions that align with the task requirements.

    Zero-shot ReAct is useful in scenarios where labeled data is scarce or expensive to obtain, as it leverages the model's pre-trained knowledge and generalization capabilities to perform tasks without explicit training. It is particularly effective in tasks that require logical reasoning, planning, and decision-making.

