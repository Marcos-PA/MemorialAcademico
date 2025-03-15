# *Analysis of the Effectiveness of Large Language Model Feature in Source Code Defect Detection*

He, Tao; Yang, Meini; Hu, Wei; Chen, Yun. *"Analysis of the Effectiveness of Large Language Model Feature in Source Code Defect Detection,"* in *3rd International Conference on Artificial Intelligence and Computer Information Technology (AICIT), 2024.* 
IEEE. doi: [10.1109/AICIT62434.2024.10730232](https://doi.org/10.1109/AICIT62434.2024.10730232)

## 1. Fichamento de Conteúdo

O artigo investiga a aplicação de Modelos de Linguagem de Grande Escala ( do inglês *Large Language Models* - LLMs) na detecção de defeitos em código-fonte. Os autores avaliam como os *outputs* desses modelos podem servir como características adicionais em algoritmos de aprendizado de máquina, melhorando a eficácia na identificação de erros.

Os experimentos foram conduzidos em um conjunto de dados de 150.000 arquivos de *JavaScript* obtidos de projetos de código aberto. Desses, 100.000 arquivos foram utilizados para treinamento e 50.000 para testes. Três tipos de defeitos foram analisados: erros na ordem de parâmetros de funções, erros nos parâmetros de operadores binários e uso incorreto de operadores binários.

Para avaliar a contribuição dos LLMs, diferentes técnicas de *prompting* foram testadas: *zero-shot*, *few-shot* e *Chain-of-Thought (CoT)*. O modelo de aprendizado de máquina utilizado foi uma Máquina de Vetores de Suporte ( do inglês *Support Vector Machine* - SVM), alimentada com características tradicionais extraídas do código (nomes de funções, tipos e ordem de parâmetros, operadores binários) e com a saída dos LLMs.

Os resultados experimentais demonstram que a introdução de características geradas por LLMs melhora a precisão da detecção de defeitos, com *few-shot prompting* apresentando o melhor desempenho. A adição dessas características melhorou significativamente a detecção de erros, especialmente os relacionados à ordem de parâmetros e ao uso de operadores binários.

## 2. Fichamento Bibliográfico

* **Uso de LLMs na detecção de defeitos**: A saída dos modelos de linguagem pode ser utilizada como característica adicional em modelos de aprendizado de máquina para aumentar a precisão na identificação de defeitos (página 3).
* **Técnicas de *prompting* analisadas**: O estudo compara *zero-shot*, *few-shot* e *Chain-of-Thought prompting*, sendo que o *few-shot* apresentou os melhores resultados (página 5).
* **Zero-shot prompting**: Avalia a capacidade do LLM de identificar defeitos sem exemplos prévios, apenas com uma instrução clara (página 6).
* **Few-shot prompting**: Fornece alguns exemplos rotulados ao LLM antes de pedir uma nova classificação, melhorando significativamente o desempenho (página 7).
* **Chain-of-Thought (CoT) prompting**: Induz o LLM a explicar seu raciocínio passo a passo, resultando em previsões mais interpretáveis (página 7).
* **Resultados experimentais**: A integração de saídas dos LLMs aumentou a precisão da detecção de erros, principalmente ao usar *few-shot prompting* (página 8).

### Tabela comparativa de precisão na detecção de defeitos

| Método | Erro de Ordem de Parâmetros | Erros em Operadores Binários |
|---------|----------------------------|----------------------------|
| Características tradicionais | 31% | 43% |
| Tradicionais + LLM (*zero-shot*) | 35% | 50% |
| Tradicionais + LLM (*few-shot*) | 39% | 56% |
| Tradicionais + LLM (*CoT*) | 38% | 54% |

* **Sugestões para pesquisas futuras**: Explorar defeitos que exigem um contexto de código mais amplo e avaliar LLMs especializados para análise de código (página 9).

## 3. Fichamento de Citações

* _"Adding feature from large language model to machine learning models can enhance the effectiveness of source code defect detection."_ (página 10)
* _"Among different strategies for constructing prompt words, few-shot prompting shows relatively better performance."_ (página 11)
* _"Machine learning models that integrate outputs from large language models demonstrate improved accuracy in identifying JavaScript code defects."_ (página 12)
* _"Traditional methods of source code defect detection are insufficient to meet the increasing demand for software security testing."_ (página 13)
* _"Future research should focus on analyzing defects that require a broader context and evaluating specialized LLMs for code analysis."_ (página 14)

