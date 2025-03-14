# On Evaluating the Efficiency of Source Code Generated by LLMs

Niu, Changan; Zhang, Ting; Li, Chuanyi; Luo, Bin; Ng, Vincent. "On Evaluating the Efficiency of Source Code Generated by LLMs," in AI Foundation Models and Software Engineering (FORGE ’24), April 14, 2024, Lisbon, Portugal. ACM, New York, NY, USA, 5 pages. doi:
[10.1145/3650105.3652295](https://doi.org/10.1145/3650105.3652295)

## 1. Fichamento de Conteúdo

O artigo investiga a eficiência do código gerado por Modelos de Linguagem de Grande Escala (LLMs), indo além da mera avaliação de correção. Para isso, os autores realizam experimentos utilizando benchmarks como HumanEval, MBPP e um conjunto de problemas do LeetCode.
As métricas analisadas incluem tempo de execução e a taxa de aceitação dos códigos gerados. Além disso, o estudo explora diferentes técnicas de _prompting_ para otimizar a eficiência dos códigos gerados, demonstrando que abordagens em múltiplas etapas melhoram os resultados.
Os achados sugerem que a eficiência do código não está diretamente relacionada ao tamanho do modelo ou à taxa de acerto inicial. Como contribuição, os autores propõem um novo benchmark baseado no LeetCode e discutem estratégias para guiar LLMs na geração de código mais eficiente.

## 2. Fichamento Bibliográfico

* **Avaliação de eficiência**: A pesquisa propõe que a avaliação de código gerado por LLMs deve considerar não apenas sua correção, mas também sua eficiência em tempo de execução (página 103).
* **Benchmarks utilizados**: O estudo utiliza os conjuntos HumanEval, MBPP e LeetCodeEval para mensurar a eficiência do código gerado pelos modelos (página 104).
* **Influência do _prompting_**: Diferentes abordagens de _prompting_ foram testadas para gerar código mais eficiente, sendo que abordagens em múltiplas etapas produziram melhores resultados (página 105).
* **Resultados experimentais**: Os modelos GPT-4 e DeepSeek Coder mostraram desempenho superior na geração de código eficiente, mas o tamanho do modelo não foi um fator determinante (página 106).
* **Impacto na produtividade**: Melhorar a eficiência do código gerado pode reduzir o tempo de desenvolvimento e otimizar a aceitação dos códigos por desenvolvedores (página 106).

## 3. Fichamento de Citações

* _"More efficient code can lead to higher performance and execution efficiency of programs and software completed by LLM-assisted programming."_
* _"The ability to generate correct code is not positively correlated with the ability to generate efficient code."_
* _"Step-by-step prompting could make LLMs generate more efficient code, especially on complex problems."_
* _"We propose a LeetCode-based benchmark which provides a reference point for comparing the correctness and efficiency of more complex code."_
* _"Training strategy and data have an impact on the efficiency of the generated code."_
