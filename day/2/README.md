# Day 2

On day 2, I wanted to deep dive into a single feature of LangChain: [prompt templates](https://python.langchain.com/docs/modules/model_io/prompts/). While reading through the [source code](https://github.com/langchain-ai/langchain/blob/d136925c49868bc24513d7a249b2d085b9c5d06a/libs/core/langchain_core/prompts/__init__.py#L11-L25), I found many different types of prompt templates:

```
    BasePromptTemplate --> PipelinePromptTemplate
                           StringPromptTemplate --> PromptTemplate
                                                    FewShotPromptTemplate
                                                    FewShotPromptWithTemplates
                           BaseChatPromptTemplate --> AutoGPTPrompt
                                                      ChatPromptTemplate --> AgentScratchPadChatPromptTemplate



    BaseMessagePromptTemplate --> MessagesPlaceholder
                                  BaseStringMessagePromptTemplate --> ChatMessagePromptTemplate
                                                                      HumanMessagePromptTemplate
                                                                      AIMessagePromptTemplate
                                                                      SystemMessagePromptTemplate
```

For just one day of learning, let's focus on two fundamental prompts: `PromptTemplate` and `ChatPromptTemplate`.

## Notebooks

### 1-deep-dive-into-PromptTemplate.ipynb

Explore the functionalities and applications of the `PromptTemplate` class. I begin with a simple prompt template without any variables, then move into templates with input variables. One interesting topic in this notebook is the discovery of partial prompts -- I didn't know langchain supported these, but they are quite powerful!

Nothing too ground-breaking here, but these are the fundamental building blocks needed to understand the rest of the library. Also at the end of the notebook there is an optional section where I use a `PromptTemplate` to interact with the `mistral-7b-openorca` model. Check it out if you are a "hands-on" learner!


### 2-deep-dive-into-ChatPromptTemplate.ipynb

Simulate a chat with `ChatPromptTemplate`, then attempt to use it with the `mistral-7b-openorca`. It doesn't work quite like I expected, but I assume this is the fault of the model and not the prompt.