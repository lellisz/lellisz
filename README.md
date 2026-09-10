<div align="center">

<img src="https://github.com/user-attachments/assets/09843cec-05ca-4138-9dec-167b4a856eea" width="100%" alt="banner"/>

<br>

<img src="https://readme-typing-svg.demolab.com/?font=IBM+Plex+Mono&size=24&duration=3200&pause=1500&color=D64545&center=true&vCenter=true&width=650&lines=Felipe+Lelis" alt="typing-svg"/>

### <img src="https://github.com/user-attachments/assets/3de1e6c0-e3f9-4e10-9a6b-6cc1edff8cc5" height="26" alt="技術"/> &nbsp;·&nbsp; <img src="https://readme-typing-svg.demolab.com/?font=IBM+Plex+Mono&size=20&duration=2600&pause=1200&color=D64545&center=true&vCenter=true&width=180&height=30&lines=AI+Engineer" alt="AI Engineer"/>

</div>

<br>

<div align="center"><img src="https://github.com/user-attachments/assets/76692d9e-5767-4eb9-952d-2a4a573ee4d5" height="24" alt="匠 whoami"/></div>

```txt
Felipe Lelis

estudo engenharia de computação na unisagrado.
exploro inteligência artificial e sistemas complexos,
com interesse em agentes, emergência e arquiteturas distribuídas.
fora do código, minha curiosidade se estende à computação,
cosmologia e astrofísica — diferentes maneiras de investigar
como sistemas complexos dão origem à ordem.
```

<div align="center"><img src="https://github.com/user-attachments/assets/f3d0b9e6-7173-4949-b676-93738de96647" height="24" alt="匠 building"/></div>

```txt
multi-agent systems.
claude api · mcp · aws bedrock.

software engineering.
```

<div align="center">

<img src="https://img.shields.io/badge/-Python-0D1117?style=flat-square&logo=python&logoColor=D64545" alt="Python"/> <img src="https://img.shields.io/badge/-TypeScript-0D1117?style=flat-square&logo=typescript&logoColor=D64545" alt="TypeScript"/> <img src="https://img.shields.io/badge/-C-0D1117?style=flat-square&logoColor=D64545" alt="C"/>
&nbsp;·&nbsp;
<img src="https://img.shields.io/badge/-LangGraph-0D1117?style=flat-square&logoColor=D64545" alt="LangGraph"/> <img src="https://img.shields.io/badge/-LangChain-0D1117?style=flat-square&logo=langchain&logoColor=D64545" alt="LangChain"/>
&nbsp;·&nbsp;
<img src="https://img.shields.io/badge/-Claude_API-0D1117?style=flat-square&logo=anthropic&logoColor=D64545" alt="Claude API"/> <img src="https://img.shields.io/badge/-MCP-0D1117?style=flat-square&logoColor=D64545" alt="MCP"/> <img src="https://img.shields.io/badge/-AWS-0D1117?style=flat-square&logo=amazonaws&logoColor=D64545" alt="AWS"/> <img src="https://img.shields.io/badge/-Cloud-0D1117?style=flat-square&logoColor=D64545" alt="Cloud"/>

</div>

<br>

## <img src="https://github.com/user-attachments/assets/c6878a10-7db6-4c30-aebe-bf8546a5d8fe" height="20" alt="侍"/> projetos selecionados

<br>

**[rag-local-ollama-chroma](https://github.com/lellisz/rag-local-ollama-chroma)**
RAG local sem framework — retrieval híbrido combinando **BM25** e busca vetorial por cosine similarity, fundidos por weighted score fusion, 100% on-device. Chunking configurável (fixed-size + overlap, testado contra chunking semântico), embeddings gerados via **Ollama** e indexados em **ChromaDB** (HNSW, tunado em ef_construction/M), com reranking opcional por cross-encoder. Cada estágio — chunking, embedding, retrieval, fusion, reranking — implementado e instrumentado manualmente (latência e recall@k logados por etapa), sem LangChain/LlamaIndex de por meio. Projeto de validação para a certificação **AWS AIF-C01**, construído para expor o que cada camada de um RAG stack realmente contribui pro resultado final.
`Python` `Ollama` `ChromaDB` `HNSW` `BM25` `Reranking` `RAG`

<br>

**[lora-portfolio-report](https://github.com/lellisz/lora-portfolio-report)**
Fine-tuning com **LoRA** (rank baixo, alpha proporcional, adapters aplicados às projeções q/v da camada de attention) sobre modelo base quantizado em 4-bit, otimizado para custo de treino em GPU única. Avaliação multi-agente do resultado — um agente audita fidelidade ao prompt, outro coerência textual, outro alucinação factual, cada um via LLM-as-judge com rubrica própria — scores agregados e comparados par a par (pairwise) contra o modelo base, no lugar de métricas isoladas como BLEU/ROUGE, que penalizam variação lexical válida.
`Python` `LoRA` `PEFT` `Quantization` `LLM-as-Judge`

<br>

**incident-copilot** <sub>· em desenvolvimento</sub>
Agente de resposta a incidentes modelado como state graph em **LangGraph** — cada nó representa uma etapa do playbook (triagem, diagnóstico, proposta de ação, aprovação), com checkpointing em **Postgres + pgvector** garantindo retomada exata do estado após falha ou timeout. Retrieval híbrido (vetor + full-text) sobre a base de runbooks, fundido via Reciprocal Rank Fusion, e reranking por LLM-as-judge antes de qualquer ação ser proposta — nenhuma ação chega ao operador sem essa camada de verificação. Modelos locais (Ollama) e cloud (Gemini, Bedrock Claude) coexistem por nó do grafo, cada um escolhido pelo trade-off custo/latência/qualidade daquela etapa específica — não por padrão fixo — com fallback automático para o modelo cloud quando a confiança do modelo local cai abaixo do threshold.
`Python` `LangGraph` `Postgres/pgvector` `RRF` `AWS Bedrock` `Human-in-the-Loop`

<br>

## <img src="https://github.com/user-attachments/assets/e58413f3-feec-4d83-8bce-a09a0ef2d917" height="20" alt="学"/> princípios

> "Entities should not be multiplied beyond necessity."
> — William of Ockham

> "Every genuine test of a theory is an attempt to falsify it."
> — Karl Popper

> "If thou art pained by any external thing, it is not this thing that disturbs thee, but thy own judgement about it."
> — Marcus Aurelius, *Meditations* VIII.47

<br>
<div align="center">

[![LinkedIn](https://img.shields.io/badge/-felipe--lelis-0D1117?style=for-the-badge&logo=linkedin&logoColor=D64545)](https://linkedin.com/in/felipe-lelis-752790375)
[![GitHub](https://img.shields.io/badge/-lellisz-0D1117?style=for-the-badge&logo=github&logoColor=D64545)](https://github.com/lellisz)

<sub><img src="https://github.com/user-attachments/assets/31a88bc0-9dfd-4d63-aa3e-28cbd36297a6" height="16" alt="道"/> — o caminho importa mais que o atalho</sub>

</div>
