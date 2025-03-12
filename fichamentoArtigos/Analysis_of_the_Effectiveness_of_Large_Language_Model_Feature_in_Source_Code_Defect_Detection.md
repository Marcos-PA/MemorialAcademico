# Analysis of the Effectiveness of Large Language Model Feature in Source Code Defect Detection

He, Tao; Yang, Meini; Hu, Wei; Chen, Yun. "Analysis of the Effectiveness of Large Language Model Feature in Source Code Defect Detection," in 3rd International Conference on Artificial Intelligence and Computer Information Technology (AICIT), 2024. 
IEEE. doi: [10.1109/AICIT62434.2024.10730232](https://doi.org/10.1109/AICIT62434.2024.10730232)

## 1. Fichamento de Conteúdo

O artigo investiga a aplicação de Modelos de Linguagem de Grande Escala (LLMs) na detecção de defeitos em código-fonte. Os autores avaliam como os outputs desses modelos podem servir como características adicionais em algoritmos de aprendizado de máquina,
melhorando a eficácia na identificação de erros. Os experimentos foram realizados em um conjunto de dados de JavaScript, onde diferentes técnicas de _prompting_ foram testadas: _zero-shot_, _few-shot_ e _Chain-of-Thought_.
Os resultados mostram que a adição das características geradas por LLMs melhora a precisão da detecção de defeitos, sendo o _few-shot prompting_ a estratégia mais eficaz. O estudo conclui que LLMs podem complementar abordagens tradicionais de análise estática e dinâmica na identificação de defeitos,
embora ainda existam desafios relacionados ao contexto e à complexidade dos erros analisados.

## 2. Fichamento Bibliográfico

* **Uso de LLMs na detecção de defeitos**: A saída dos modelos de linguagem pode ser utilizada como característica adicional em modelos de aprendizado de máquina para aumentar a precisão na identificação de defeitos (página 2).
* **Técnicas de _prompting_ analisadas**: O estudo compara _zero-shot_, _few-shot_ e _Chain-of-Thought prompting_, sendo que o _few-shot_ apresentou os melhores resultados (página 5).
* **zero-shot**: refere-se à capacidade de um grande modelo de linguagem de concluir uma tarefa específica sem ter visto nenhum dado relacionado a essa tarefa anteriormente.
* **few-shot**: O prompt de poucos disparos pode melhorar o desempenho ao fornecer exemplos de demonstração dentro dos prompts para aprendizagem de contexto.
* **Chain-of-Thought**: é um método que incentiva grandes modelos de linguagem a explicar seus processos de raciocínio. Ele auxilia na compreensão e avaliação das capacidades e limitações do modelo
* **Resultados experimentais**: A introdução de características dos LLMs melhorou significativamente a detecção de erros como ordem de parâmetros, erros em operadores binários e uso incorreto de operadores (página 6).
* **Impacto do _prompting_**: Modelos que receberam exemplos durante o _prompting_ foram mais eficazes na predição de defeitos do que aqueles submetidos a _zero-shot prompting_ (página 7).
* **Sugestões para pesquisas futuras**: Investigar defeitos mais complexos que exigem análise contextual profunda e avaliar o desempenho de LLMs especializados em código-fonte (página 8).

## 3. Fichamento de Citações

* _"Adding feature from large language model to machine learning models can enhance the effectiveness of source code defect detection."_
* _"Among different strategies for constructing prompt words, few-shot prompting shows relatively better performance."_
* _"Machine learning models that integrate outputs from large language models demonstrate improved accuracy in identifying JavaScript code defects."_
* _"Traditional methods of source code defect detection are insufficient to meet the increasing demand for software security testing."_
* _"Future research should focus on analyzing defects that require a broader context and evaluating specialized LLMs for code analysis."_
