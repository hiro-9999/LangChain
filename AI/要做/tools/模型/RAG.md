## gemini embedding 2
https://www.youtube.com/watch?v=8f2kMpOqF04

https://ledge.ai/articles/google_gemini_embedding_2_multimodal_embedding_model

https://ai.google.dev/gemini-api/docs/embeddings

https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-embedding-2/

## openrouter
LLMs 大模型
https://openrouter.ai/

## pinecone
https://www.pinecone.io/

```
1. 综合评价最好（最省心）：Pinecone
如果你不想管理任何服务器，只想通过 API 调用来实现 AI 功能，它是首选。

Pinecone 是一个专门为人工智能（AI）设计的 向量数据库 (Vector Database)。

在传统的数据库（如 MySQL）里，你搜索的是“关键词”；而在 Pinecone 这种向量数据库里，搜索的是“意思”（语义）。它是目前大模型（LLM）开发生态中最常用的基础设施之一。

以下是它的核心用途和应用场景：

1. 给 AI 提供“长期记忆” (RAG)
这是目前最火的用途。大模型（如 ChatGPT）的知识是有截止日期的，且无法记住你私有的长篇文档。

怎么做： 你把公司的文档、书籍或笔记转成“向量”（一串数字），存进 Pinecone。

效果： 当你问 AI 问题时，它先去 Pinecone 里搜索最相关的片段，再把这些片段交给大模型。这就是 RAG（检索增强生成），能让 AI 回答极其专业且实时的内容。

2. 语义搜索 (Semantic Search)
传统的搜索靠匹配字面单词（搜“猫”可能找不到“小咪”），而 Pinecone 靠匹配含义。

用途： 即使搜索者用的词不对，只要意思相近，Pinecone 就能精准找到结果。适用于企业内部知识库、电商商品搜索等。

3. 推荐系统 (Recommendation Systems)
原理： 把用户的兴趣和物品（电影、音乐、商品）都转化为向量。

用途： 快速计算出哪些物品和用户的兴趣最“接近”，从而实现像抖音、小红书那样的精准推荐。

4. 异常检测与图像检索
图像搜索： 你上传一张图片，它能在一秒内从几百万张图片里找出视觉上最相似的。

安全反欺诈： 识别行为模式异常的向量，用于金融反欺诈。

优点： 全托管（Serverless），上线极快，性能非常稳定，几乎是开发者构建 RAG（检索增强生成）应用的标准配置。

缺点： 价格随数据量增加而变得昂贵，且不支持本地部署（只能用他们的云）。

2. 开源/性能平衡最好：Qdrant
目前在开发者社区口碑极佳，尤其是在欧洲和追求性能的团队中。

优点： 使用 Rust 编写，速度极快且极其节省内存。它的元数据过滤（Metadata Filtering）功能非常强大（比如：在海量数据中只搜索“2025年之后”的向量）。

缺点： 相比 Pinecone，如果你选择自托管，需要一定的运维能力。

3. 企业级/超大规模最好：Milvus
如果你有超过十亿级别的向量数据，Milvus 是目前最稳妥的选择。

优点： 专门为分布式大规模扩展设计，支持 GPU 加速搜索，性能上限极高。其商业版 Zilliz Cloud 提供了类似 Pinecone 的托管服务。

缺点： 架构复杂，自建集群的门槛很高（需要管理很多组件）。

4. 功能最丰富（混合搜索）：Weaviate
如果你的应用不仅需要查向量，还需要查关键词（类似 Google 的混合搜索）。

优点： 内置了向量化模型接口，你可以直接把文本丢进去，它帮你转成向量。支持 GraphQL 查询，对开发者非常友好。

缺点： 纯向量搜索的速度略慢于 Qdrant。
```

## n8n
🚧 開始使用 n8n 構建自動化! 👇
https://n8n.partnerlinks.io/fwp82h8azh6k

## look 
https://www.youtube.com/watch?v=6s_Z9Tl0sHU


## ChatGPT 最新推出的 Image 2.0 



## AI監控 TikTok 爆款影片 → 自動找到相關股票
https://www.youtube.com/watch?v=th_ebf93k-c


## Claude Code + Vibe Coding 太猛了！80分鐘打造完整 RAG AI 網站
這支影片，我用 1 小時 20 分鐘，完整帶你用 Claude Code + Vibe Coding 的方式，從 0 打造一個真正可用的多功能 RAG 網站。
你將學會：
如何用 Claude Code 做 Web Coding
用 Vibe Coding 的方式快速生成前後端架構
建立多功能 RAG 系統（知識庫 / 文件問答 / 多資料整合）
打造可部署、可擴展的 AI Web App
這不是單純 Demo，而是完整實戰流程。即使你是新手小白，只要跟著操作，你可以自己做出一個真正屬於你的 AI 網站。
這是一種全新的寫程式方式 —— Vibe Coding。
https://github.com/harryleemedia/claude-code-agentic-rag-masterclass
https://supabase.com/
https://smith.langchain.com/
https://openrouter.ai/
https://mistral.ai/
https://dashboard.cohere.com/
https://app.tavily.com/
https://vercel.com/
