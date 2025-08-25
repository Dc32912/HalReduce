# HalReduce: An Agent Framework for Reducing Hallucinations in LLMs

HalReduce is an intelligent Agent system designed to **reduce hallucinations in Large Language Models (LLMs)**.  
It integrates **Retrieval-Augmented Generation (RAG)**, **Prompt Optimization**, **Tool Invocation**, and **Multi-Model Verification (MMV)** into a unified workflow.  
The system is implemented with LangChain, and experiments are conducted on the HaluEval dataset.

---

##  Features

- **Retrieval-Augmented Generation (RAG)**  
  Retrieve relevant knowledge from a local vector database (Chroma) and supplement with real-time web search.

- **Prompt Optimization**  
  Use structured prompts with explicit rules to regulate reasoning steps and ensure clear, interpretable outputs.

- **Tool Function**  
  Seamless integration of external tools such as:
  - `get_info_from_local_db`: retrieve knowledge from Chroma
  - `search`: real-time search using Google Serper API
  - `multi_model_verify`: perform multi-model consistency verification

- **Multi-Model Verification (MMV)**  
  Multiple LLMs (GPT-3.5, GPT-4, Claude) independently judge the same answer, then majority voting determines the final decision.

---
