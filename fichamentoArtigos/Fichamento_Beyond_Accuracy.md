# Beyond Accuracy: Evaluating Source Code Capabilities in Large Language Models for Software Engineering

Velasco, Alejandro. "Beyond Accuracy: Evaluating Source Code Capabilities in Large Language Models for Software Engineering," in 2024 IEEE/ACM 46th International Conference on Software Engineering: Companion Proceedings (ICSE-Companion ’24), April 14–20, 2024, Lisbon, Portugal. ACM, New York, NY, USA. 
doi: [10.1145/3639478.3639815](https://doi.org/10.1145/3639478.3639815)

## 1. Fichamento de Conteúdo

O artigo discute a necessidade de avaliar Modelos de Linguagem de Grande Escala (LLMs) para Engenharia de Software além das métricas tradicionais de acurácia. O autor propõe novas abordagens de interpretabilidade para entender melhor o desempenho desses modelos em tarefas como compreensão de código, geração e reparo de programas.
O estudo destaca a limitação das métricas existentes, como BLEU e CodeBLEU, que não capturam adequadamente propriedades semânticas como confiabilidade, manutenibilidade e robustez. O trabalho sugere uma abordagem baseada na Teoria das Categorias e Inferência Causal para modelar e avaliar as capacidades dos LLMs, classificando-as em linguísticas, semânticas e de qualidade.
Como contribuição prática, o autor propõe ferramentas para avaliar e detectar erros, visando fornecer insights mais úteis para desenvolvedores e pesquisadores da área.

## 2. Fichamento Bibliográfico

* **Métricas limitadas**: Métricas tradicionais de avaliação de modelos de linguagem, como BLEU e CodeBLEU, não capturam aspectos semânticos do código gerado (página 162).
* **Classificação das capacidades dos LLMs**: O estudo propõe três categorias principais para avaliar modelos: linguísticas, semânticas e de qualidade (página 163).
* **Uso da Teoria das Categorias**: A modelagem semântica do código é realizada por meio da Teoria das Categorias e do Embedding de Yoneda (página 163).
* **Impacto na Engenharia de Software**: A pesquisa visa melhorar a confiabilidade e manutenibilidade do código gerado por IA, propondo novos métodos de análise (página 164).
* **Desenvolvimento de ferramentas**: O estudo prevê a criação de ferramentas para interpretar e avaliar modelos, ajudando desenvolvedores na escolha e utilização de LLMs para tarefas de programação (página 164).

## 3. Fichamento de Citações

* _"Current canonical metrics fall short of offering insights into the extent to which the evaluated models learn meaningful semantic information from the source code."_
* _"By considering these enriched semantic aspects in the evaluation of proposed architectures, we can improve future research in deep learning for software engineering."_
* _"We define three types of source code capabilities: Linguistic, Semantic, and Quality."_
* _"Our final goal is to design, develop, and publish usable tools to incorporate the previous elements for error detection and evaluation of LLMs for code."_
* _"A key feature of our tools will be their ability to translate complex model decisions into human-understandable knowledge in terms of source code capabilities."_
