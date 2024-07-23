# Generative AI Project 

## Day 1: Project Introduction [Video](https://www.youtube.com/watch?v=LzaTRANbEYk)
* providers/services you can use (if you want to create robust applications & to get a quick response from llms)
>-> OpenAI
>
>-> AWS Bedrock
>
>-> GCP Vertex
>
>-> Azure openAI/LLMOps

* Few milestone in large language model
> * Bard
>
> * GPT
>
> * XLM
>
> * T5
> 
> * M2M-100

* What is LLMs?
> A large language model is a trained deep learning model that understands and generate text in a human like fashion.
> 
> LLMs are good at understanding and generating human language

* traditional NLP models
> RNN
>
> LSTM
> 
> GRU
>
> encoder-decoder/attention mechanism -- Transformer

* Why we call it Large Language Model?
> Because of the size and complexity of the Neural Network as well as the size of the dataset that it was trained on.
> 
> Researchers started to make these models large and trained on huge datasets.
>
> That they started showing impressive results like understanding complex Natural Language and gerarating language more eloquently than ever. 

* What makes LLM so Powerful?
> In case of LLM, one model can be used for a whole variety of tasks like:
> > Text generation, Chatbot, summarizer, translation, code generation & so on ...
> So, LLM is subset of Deep Learning & it has some properties merge with Generative AI

About the open source models:[Open LLMs -- Github](https://github.com/eugeneyan/open-llms)

* What can LLMs be used for?
> Text Classification
>
> Text Generation
>
> Text Summariztion
> 
> Conversation AI like chatbot, Question Answering
>
> Speech recognition and Speech identification
>
> Spelling Corrector

* How ChatGPT was trained?
> Internally using a LLM which is gpt-3.5 or gpt-4. It has trained on a large amount of data which is available all over the internet.
> > 1. Generative pre-training
> > 2. Supervised fine-tuning
> > 3. Reinforcement learning

* 工具介紹
> [GEMINI](https://gemini.google.com/app)

* 開始建立 Project -- 只有初始化，在下一個 Lecture 完成主要部分
> [Chatbot-Implementation-Using-Chainlit](https://www.youtube.com/watch?v=MPviIidzBv4)


## Day 2: Chatbot Implementation Using Chainlit [Video](https://www.youtube.com/watch?v=MPviIidzBv4)
> Github -- [Chatbot-Implementation-Using-Chainlit](https://www.youtube.com/watch?v=MPviIidzBv4)

## Day 3: Chatbot Implementation Using Telegram [Video]()
> Github -- [Chatbot-Implementation-using-Telegram](https://github.com/henrykohl/Chatbot-Implementation-using-Telegram)


## Day 4: RAG Application Using OpenSource Framework [Video](https://www.youtube.com/watch?v=2lBPs2bb7sw)
> [Simple_RAG_Demo.ipynb](https://github.com/henrykohl/Machine-Learning-demo-repo/blob/master/NaturalLanguage/genaiproj-ineuron/Simple_RAG_Demo.ipynb)
> [stats1.pdf](https://github.com/henrykohl/Machine-Learning-demo-repo/blob/master/NaturalLanguage/genaiproj-ineuron/stats1.pdf)
>
> [statsb.pdf](https://github.com/henrykohl/Machine-Learning-demo-repo/blob/master/NaturalLanguage/genaiproj-ineuron/statsb.pdf)

## Day 5: Realtime Powerful RAG Pipeline using Neo4j and Langchain [Video](https://www.youtube.com/watch?v=XrQvCpjqsvo)
> [Powerful_RAG_demo_with_Neo4j.ipynb](https://github.com/henrykohl/Machine-Learning-demo-repo/blob/master/NaturalLanguage/genaiproj-ineuron/Powerful_RAG_demo_with_Neo4j.ipynb)
>
> [Copy_of_RAG_With_Knowledge_graph(Neo4j).ipynb](https://github.com/henrykohl/Machine-Learning-demo-repo/blob/master/NaturalLanguage/genaiproj-ineuron/Copy_of_RAG_With_Knowledge_graph(Neo4j).ipynb)


* Tabular Database --> Structured Data . Schema
> MYSQL

* Unstructured Database --> Dict format . Key-value
> MongoDB

* Graph Database --> Tree . graph
> Neo4j

* 3 Query search -- Combine result -- Get (the accurate answer from your large langue model)

* Libraries used to implement the particular system here:
> Langchain (o) / LlamaIndex (x)
>
> Langchain community
> 
> OpenAI, OpenAI embedding, OpenAI LLM
> 
> Vector DB：Neo4j graph
> 
> Data：Wikipedia

user----(question)---->|////Document////| (D)

(D)----(graph search)---->|knowledge graph| (KG)
> 1>
2> (D)----(keyword search)---->|Docs of unstructure data| (UD)
> 2>
(D)----(vector search)---->|Docs of unstructure data| (UD)
> 3>

1>+2>+3> ---|combine source|--->|LLM|--->Response Context


## Day 6: Powerful RAG Using Hybrid Search [Video](https://www.youtube.com/watch?v=6njA_tXdgww)
> [Hybrid_Search_RAG.ipynb](https://github.com/henrykohl/Machine-Learning-demo-repo/blob/master/NaturalLanguage/genaiproj-ineuron/Hybrid_Search_RAG.ipynb)


+-------------------------------------Hybrid Search RAG-------------------------------------+

Weaviate - Vector DB - Cloud version

LLM - HuggingFace

+-------------------------------------------------------------------------------------------+

補充參考:
[Langchain - Mistral 7B 模型實作](https://medium.com/@pang2258/55ce9eedb63a)

[用 bitsandbytes、4 比特量化和 QLoRA 打造親民的 LLM](https://www.cnblogs.com/huggingface/p/17816374.html)

[即用的 pipelines -- 來自 transformers](https://transformers.run/c2/2021-12-08-transformers-note-1/)

[【LangChain】Prompts之Prompt templates](https://cloud.baidu.com/qianfandev/topic/267844)

## Day 7: Deployment of LLM Application [Video](https://www.youtube.com/watch?v=y4F139pLHGI)

Generative AI：
> |LLM| 包含
> 
>  ------> Commerical
>
>  ------> Open Source

Cloud Providers:
> -> OpenAI
> 
> -> AWS Bedrock
> 
> -> GCP Vertex
> 
> -> Azure openAI/LLMOps

---

Application - Open Source LLM

******** **Amazon sagemaker** ********

> 架構 :
> 
> [ModelBuilder]->[Model Artifacts]->[AWS S3 Bucket]=>[AWS Sagemaker]<=[Model deploy]-->[AWS Sagemaker model End point] ( * )
> ~ ~ ~ work flow ~ ~ ~
>
> user  ---request---> ( * )
>
> user <---response--- ( * )

Required two things / two credential 
> AWS Access key
> 
> AWS Secret access key

---

補充課程：
> [LLMOps End to End Project](https://www.youtube.com/playlist?list=PLmQAMKHKeLZ_77CBNeOoUyZUMzlqX-fpe)
>
> * EC2 instance (可以用在 the next deployment process--the commercial model)
>
> [End to End DL project implementation](https://www.youtube.com/playlist?list=PLmQAMKHKeLZ_WWr8QBxKbMTE4tpwb4f1q) (Bappy 說 此標題 不太正確)

---
* 開始部署 application -- source:
> [Medical-Disease-Analysis-using-GPT4-Vision](https://github.com/henrykohl/Medical-Disease-Analysis-using-GPT4-Vision)

* 在 AWS 建立 EC2 instance
> `Launch an instance`
>
> Name 是 `llm deploy`
> 
> **Quick Start** 用 `Ubuntu`
>
> Amazon Machine Image(AMI) 用 `Ubuntu Server 24.04 LTS (HVM), SSD Volume Type`
>
> Instance type 用 `t2.large`
>
> Key pair name 用 `mchatbot` (這是以前建立過的，其 pem 檔還保留)
>
> 勾選 `Allow HTTPS traffic from the internet` 與 `Allow HTTP traffic from the internet`
>
> **Configure storage** 用 `30` GB

* 建立了 Instance 後，Connect 連線此 EC2
> ```bash
> sudo apt update
> 
> sudo apt-get update
> 
> sudo apt upgrade -y
> 
> sudo apt install curl unzip tar make sudo vim wget -y
> 
> git clone https://github.com/henrykohl/Medical-Disease-Analysis-using-GPT4-Vision.git
>
> cd Medical-Disease-Analysis-using-GPT4-Vision
> ```

* 建立/完成 `.env`
> ```bash
> touch .env
>
> vim .env
> > OPENAI_API_KEY = "......................"
> ```

* 繼續在 EC2 instance 操作
> ```bash
> sudo apt install python3-pip
> 
> pip3 install -r requirements.txt
> ```

* 安裝 requirements.txt 遇到錯誤 `error: externally-managed-environment`
> ```bash
> sudo apt install python3-venv
>
> python3 -m venv .venv
> 
> source .venv/bin/activate
>
> pip3 install -r requirements.txt
> ```

* 設定 **Security** -> Security group -> `Edit inbound rules -> `Add rule`
> Type 選 `Custom TCP`
> 
> Port range 用 `8501`
>
> Source 選 `0.0.0.0/0`

-> `Save rules` 

* 開啟 `Streamlit APP`
> ```bash
> python3 -m streamlit run StreamlitAPP.py
> ```

* 若要 `Streamlit APP` 可以 Permanent running
> ```bash
> nohup python3 -m streamlit run StreamlitAPP.py
> ```

---

進階參考--使用CICD
> [Streamlit-APP-Deploy-AWS-CICD](https://github.com/entbappy/Streamlit-APP-Deploy-AWS-CICD)
>
> [Omdena](https://www.omdena.com/) --Building AI Solutions

---
Inference 模式
> user ---> [LLM]
>
> user <--- [LLM]

RAG 模式:
> [custom data] (1)---連接--->[knowledge base] (2)<---連接---[LLM] (3)
> 
> ~ ~ ~ work flow ~ ~ ~
>
> user ---> (2) ---> (3) 
> 
> user      <---     (3) 
---
補充:
[Comparing 10+ LLMOps Tools](https://research.aimultiple.com/llmops-tools/)


