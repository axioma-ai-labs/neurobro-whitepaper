---
icon: car-battery
description: All Agents share something in common
---

# Core Technologies

## 1. Core Agents Components

Each Agent has its own functionality, sources of data, and input points for interacting with the real environment. Below is an overview of these components:

### **a) Knowledge Bases**

We utilize multiple advanced [RAG systems](https://en.wikipedia.org/wiki/Retrieval-augmented_generation) for storing & retrieving internal documents and crypto-related posts/articles/tweets, etc.

Our primary vector stores include [Weaviate](https://weaviate.io/) and [Qdrant](https://qdrant.tech/).

Agents & Core Agents use these to store and retrieve:

* Internal documents (e.g., Neurobro official documentation, this whitepaper, $BRO qualitative statistics)
* Historical crypto-related articles and tweets.
* Agent actions (e.g., posted tweets, comments, user questions).

### **b) Embeddings**

All embeddings are created using the SOTA [text-embedding-3-large](https://openai.com/index/new-embedding-models-and-api-updates/) model from OpenAI, ensuring precision and relevance for every query and operation.

### **c) APIs**

Neurobro Ecosystem integrates with both proprietary and public APIs.

* \~90% of the value visible to the public comes from proprietary APIs.
* \~10% comes from publicly available APIs (e.g., [Coingecko](https://www.coingecko.com/en/api), [DexScreener](https://docs.dexscreener.com/api/reference), [Base BlockScout](https://docs.blockscout.com/devs/apis)).

The **Neurobro Core Development Team** is dedicated to optimizing API performance and speed, ensuring a reliable and seamless experience both for users & our agents.

***

## 2. LLMs

Large Language Models form the backbone of the Neurobro AI ecosystem, powering ALL of our agents. These models provide the basic intelligence needed to understand complex inputs, generate coherent and insightful outputs, and perform highly specialized tasks with precision.

**🔸 Most used LLMs:**

* [R1 & V3](https://api-docs.deepseek.com/) **by DeepSeek**: Used for reasoning tasks.
* [**Llama 3.1 (405B)**](https://ai.meta.com/blog/meta-llama-3-1/) **by Meta**: Used for large-scale analysis and replies.
* [**GPT-4o**](https://openai.com/index/hello-gpt-4o/) **&** [**o3 Series**](https://openai.com/o1/) **by OpenAI**: Used for tasks like formatting and intent recognition.
* **Custom Fine-Tuned Models**: Open-source models fine-tuned for specialized tasks, focusing on e.g., data cleansing and Neurobro personality alignment.

***

## 3. Tools

Each agent’s workflow utilizes specific tools. A tool is defined as an external function, capability, or resource accessed by the agent to:

* Perform predefined task
* Extend abilities
* Fetch external information

**🔸 Examples of tools:**

* **Neurobro Telegram Assistant**: Answers questions about real-time $BRO financial data using DexScreener.
* **Neurobro KOL on X**: Replies to tweets mentioning "@0xNeurobro," scrapes the latest news from Binance Blog

**🔸 General tooling representation**

🔍 Tool Identification → ⚙️ Tool Execution → ✨ Response Generation

