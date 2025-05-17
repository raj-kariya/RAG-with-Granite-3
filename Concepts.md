# Large Language Models

Large Language Models (LLMs) are trained on vast datasets, but they don’t inherently include your specific data. Retrieval-Augmented Generation (RAG) addresses this limitation by integrating your data with the existing knowledge that LLMs possess. Throughout this documentation, you'll often encounter references to RAG. It's a key method used by query engines, chat engines, and agents to enhance their functionality.
In a RAG setup, your data is loaded, processed, and indexed for efficient querying. When a user submits a query, the system interacts with the index to narrow down your data to the most pertinent context. This relevant context, combined with the user's query, is then passed to the LLM, which generates a response based on this tailored information.
Whether you’re developing a chatbot or an intelligent agent, understanding RAG techniques is essential for effectively incorporating your data into the application.

## RAG Concepts
Within the RAG framework, there are five key stages, though in this lab, we'll focus on the first four. These stages are fundamental to most larger applications you might develop. The stages include:

- **Loading**: This involves bringing your data into your workflow, regardless of its source—be it text files, PDFs, websites, databases, or APIs. LlamaHub offers a wide array of connectors to facilitate this process.

- **Indexing**: This stage involves creating a data structure that enables efficient querying. For LLMs, this typically involves generating vector embeddings, which are numerical representations that capture the meaning of your data, along with various metadata strategies to ensure accurate and contextually relevant data retrieval.

- **Storing**: After indexing, it's usually important to save your index along with associated metadata to avoid the need for re-indexing in the future.

- **Querying**: Depending on your indexing strategy, there are multiple ways to utilize LLMs and LlamaIndex data structures for querying. This can include sub-queries, multi-step queries, and hybrid approaches.

- **Evaluation** : An essential stage in any workflow is evaluating how effective your approach is compared to others or when adjustments are made. Evaluation offers objective metrics to assess the accuracy, fidelity, and speed of your query responses.

<figure>
    <img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/uEQ_sNaMScgOgnNh6olKGg/stages.png" width="100%" alt="langchain">
    <figcaption><a href="https://docs.llamaindex.ai/en/stable/getting_started/concepts/">source</a></figcaption>
</figure>


