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

This is going to be an interesting day. Time to roll up my sleeves 💪 and get to coding!

## Notebooks

### 1-deep-dive-into-PromptTemplate.ipynb

Create several instances of `PromptTemplate` and perform some typical conde introspection. Test how to create a prompt with variables, and showcase partial prompts.

### 