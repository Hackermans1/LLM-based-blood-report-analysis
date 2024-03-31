### Phase 1 
Utilizing a base the GPT4All model for semantic search, which can be repeated with other models as well but this one is most friendly for consumer grade PCs. The steps are as follows:

Load GPT4All Model: Begin by loading the GPT4All model.

Retrieve and Load Documents: Utilize Langchain to retrieve documents and load them for processing.

Chunk Documents for Embeddings: Split the documents into smaller, digestible chunks suitable for embedding.

Create Vector Database with FAISS: Utilize FAISS to create a vector database with embeddings.

Perform Similarity Search: Conduct a semantic search on the vector database based on a question provided as context for the search.

Feed Question and Context to GPT4All: Provide the question and context to GPT4All via Langchain and wait for the answer.

In this process, embeddings play a crucial role. Embeddings are numerical representations of information such as text, documents, images, etc., capturing their semantic meaning. For this project, heavy GPU models are not relied upon. Instead, the Alpaca native model is downloaded, and LlamaCppEmbeddings from Langchain are utilized for embeddings.

### Phase 2 
**Finetuning** models to work better on medical reports 