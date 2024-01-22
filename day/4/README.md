# Day 4

Today, I want to review the different methods of summarizing a document with LLMs. Text summarization is an NLP task which distills a large document into a smaller, more concise one.

I am referencing a few different blog posts for my learnings today:
  * [Mastering Document Chains in LangChain | Comet](https://www.comet.com/site/blog/mastering-document-chains-in-langchain/)
  * [Summarize Large Documents in LangChain | Google](https://github.com/GoogleCloudPlatform/generative-ai/blob/main/language/use-cases/document-summarization/summarization_large_documents_langchain.ipynb)
  * [Challenges of LLM for Large Document Summarization... | Medium](https://medium.com/google-cloud/langchain-chain-types-large-document-summarization-using-langchain-and-google-cloud-vertex-ai-1650801899f6)

## Notebooks

### 1-summarize-via-stuffing.ipynb

[View Notebook](./1-summarize-via-stuffing.ipynb) &nbsp; • &nbsp; [Open Notebook in Collab](https://colab.research.google.com/github/jacobbridges/100-Days-Of-AI/blob/main/day/4/1-summarize-via-stuffing.ipynb)

This notebook covers the simplest summarization method, "Stuffing". I learn a bit about context windows, [LangChain Documents](https://github.com/langchain-ai/langchain/blob/master/libs/core/langchain_core/documents/base.py#L9), and the `load_summarize_chain()` function.

### 2-summarize-via-map-reduce.ipynb

[View Notebook](./2-summarize-via-map-reduce.ipynb) &nbsp; • &nbsp; [Open Notebook in Collab](https://colab.research.google.com/github/jacobbridges/100-Days-Of-AI/blob/main/day/4/2-summarize-via-map-reduce.ipynb)

This notebook showcases the "Map-Reduce" method of summarizing documents. I was not a huge, as it begins to feel like a [game of telephone](https://en.wikipedia.org/wiki/Chinese_whispers), but was still interesting to learn about the technique.

