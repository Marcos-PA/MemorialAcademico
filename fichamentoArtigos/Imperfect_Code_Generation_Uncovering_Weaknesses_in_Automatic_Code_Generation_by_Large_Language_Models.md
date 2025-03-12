# Imperfect Code Generation: Uncovering Weaknesses in Automatic Code Generation by Large Language Models

Lian, Xiaoli; Wang, Shuaisong; Ma, Jieping; Tan, Xin; Liu, Fang; Shi, Lin; Zhang, Li; Gao, Cuiyun. "Imperfect Code Generation: Uncovering Weaknesses in Automatic Code Generation by Large Language Models," in 2024 
IEEE/ACM 46th International Conference on Software Engineering: Companion Proceedings (ICSE-Companion ’24), April 14–20, 2024, Lisbon, Portugal. ACM. doi: [10.1145/3639478.3643081](https://doi.org/10.1145/3639478.3643081)

## 1. Fichamento de Conteúdo

O artigo investiga as fraquezas na geração automática de código por Modelos de Linguagem de Grande Escala (LLMs). Apesar dos avanços recentes, os modelos ainda apresentam falhas que comprometem a qualidade do código gerado. 
O estudo avalia três LLMs de última geração (GPT-4, CodeGeeX2 e CodeGen2.5) utilizando três conjuntos de dados amplamente empregados na pesquisa (CoNaLa, HumanEval+ e DS-1000). Os pesquisadores identificaram oito categorias principais de fraquezas,
que variam desde falhas na compreensão dos _prompts_ até o uso incorreto de APIs e redundância na geração de código. Como solução, o artigo sugere melhorias nos benchmarks e no treinamento dos modelos para mitigar esses problemas e otimizar a precisão e utilidade dos códigos gerados por IA.

## 2. Fichamento Bibliográfico

* **Categorias de fraquezas**: O estudo identifica oito principais problemas na geração de código por LLMs, incluindo _prompts_ imprecisos, falhas semânticas e uso incorreto de APIs (página 3).
* **Modelos e benchmarks analisados**: Foram avaliados três LLMs (GPT-4, CodeGeeX2 e CodeGen2.5) em três conjuntos de dados (CoNaLa, HumanEval+ e DS-1000) (página 4).
* **Impacto dos _prompts_**: A qualidade do código gerado é diretamente influenciada pela clareza e precisão dos _prompts_, sendo que _prompts_ muito complexos aumentam as taxas de erro (página 5).
* **Uso incorreto de APIs**: Erros comuns incluem parâmetros errados ou chamadas para APIs inexistentes, impactando negativamente a funcionalidade do código (página 6).
* **Sugestões de melhoria**: O estudo propõe benchmarks mais sofisticados e estratégias avançadas de treinamento para reduzir erros na geração de código (página 8).

## 3. Fichamento de Citações

* _"Despite achieving state-of-the-art performance, LLMs still generate code with significant weaknesses that need to be addressed."_
* _"Our study identifies eight distinct categories of weaknesses in code generation and highlights their prevalence across multiple benchmarks."_
* _"Inaccurate prompts lead to misinterpretations, making it nearly impossible for LLMs to generate correct source code."_
* _"We propose refining benchmarks to include API-diverse solutions and improve semantic representation of prompts to enhance code accuracy."_
* _"Gold plating and redundant code generation remain critical issues that require targeted mitigation strategies."_
