# 🐴 Mustang-ChatBot
This repository holds code for an LLM powered ChatBot for the Ford Mustang.

# 👀 Overview
This is an LLM powered AI Chatbot that has been designed to answer questions about the Ford Mustang line of sports cars. It uses [HuggingFace](https://huggingface.co/) as a provider for both the LLM and Embeddings Model. It has been written using [Python](https://www.python.org/) and [LangChain.](https://docs.langchain.com/)

This AI Chatbot uses RAG techniques to provide users with accurate information. It uses the [Ford Mustang Wikipedia page](https://en.wikipedia.org/wiki/Ford_Mustang) as a source for the RAG embedding process. It currently uses an In-Memory Vector Store, however, more scalable solutions such as a ChromaDB Vector Database is being considered.

The following Open Source Models are currently being used, both can be easily tweaked/changed for any HuggingFace Open Source Model

- Chat Model: https://huggingface.co/meta-llama/Llama-3.1-8B-Instruct 
- Embeddings Model: https://huggingface.co/model-embeddings/multi-qa-mpnet-base-dot-v1 

For detailed deep dive on this project and RAG architecture, feel free to read [this](https://medium.com/@samiur1998/creating-an-ai-powered-chatbot-using-llms-rag-langchain-and-python-4903fd786c0b) article.

# 🛠️ Setup & Usage
In order to use this application a HuggingFace API Key is necessary.

Once users have an API Key, a **.env** file must be created in the root directory and populated with the following contents:
```
HUGGINGFACEHUB_API_TOKEN=YOUR_API_KEY
HF_TOKEN=YOUR_API_KEY
```

Once the API Key has been added to the environment variables, users may begin using the ChatBot. It is worth noting that the current config of the ChatBot uses free models for both the LLM and RAG Embeddings. A different configuration choice however, may effect this.

Additionally the Application downloads a local verison of the embeddings model. This makes the embedding process alot faster and cost-effective. This is created in a local folder called **embeddings_models**. It is recommended for users to delete this folder after usage.

In order to use the application please install Python and then run the following commands:
```
python3 -m venv venv (Creates a Virtual Environment)
source venv/bin/activate (Activates Virtual Environment)
pip install -r requirements.txt (Installs Necessary Dependencies)
python3 main.py (Executes and Runs the Application)
```

# 🍴 Forking & Contributions
Users are more than welcome to both fork this repo and use the code here.

However please do take note of the following:
[**LICENSE**](https://github.com/shahLLL/Mustang-ChatBot?tab=MIT-1-ov-file)

☕☕☕**CHEERS AND THANK YOU**☕☕☕