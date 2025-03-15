# Beyond Accuracy: Evaluating Source Code Capabilities in Large Language Models for Software Engineering

Velasco, Alejandro. "Beyond Accuracy: Evaluating Source Code Capabilities in Large Language Models for Software Engineering," in 2024 IEEE/ACM 46th International Conference on Software Engineering: Companion Proceedings (ICSE-Companion ’24), April 14–20, 2024, Lisbon, Portugal. ACM, New York, NY, USA. 
doi: [10.1145/3639478.3639815](https://doi.org/10.1145/3639478.3639815)

## 1. Fichamento de Conteúdo

O artigo investiga a necessidade de avaliar *Modelos de Linguagem de Grande Escala* ( do inglês *LLMs - Large Language Models*) para engenharia de software além das métricas tradicionais de acurácia. O autor propõe novas abordagens de interpretabilidade para compreender melhor o desempenho desses modelos em tarefas como compreensão de código, geração e reparo de programas.

O estudo destaca a limitação das métricas existentes, como *BLEU* e *CodeBLEU*, que não capturam adequadamente propriedades semânticas essenciais, como confiabilidade, manutenibilidade e robustez. Para contornar essa limitação, o trabalho sugere uma abordagem baseada na *Teoria das Categorias* e *Inferência Causal* para modelar e avaliar as capacidades dos *LLMs*, classificando-as em três categorias principais:

1. **Capacidades linguísticas**: Avaliam a compreensão sintática dos modelos.
2. **Capacidades semânticas**: Medem o conhecimento de domínio embutido nas respostas.
3. **Capacidades de qualidade**: Avaliam a capacidade dos modelos de gerar código eficiente, seguro e livre de vulnerabilidades.

Além disso, o artigo propõe ferramentas para avaliar e detectar erros nos modelos, fornecendo informações mais úteis para desenvolvedores e pesquisadores.

## 2. Detalhamento do Experimento

Os experimentos foram conduzidos com foco em três objetivos principais:
1. **Compreender as informações semânticas capturadas pelos modelos**.
2. **Avaliar a eficácia dos *LLMs* na aprendizagem de tais informações**.
3. **Desenvolver ferramentas de detecção de erros para auxiliar na análise e confiabilidade dos modelos**.

### **Metodologia**
A avaliação dos modelos foi realizada em três etapas principais:

1. **Modelagem das capacidades semânticas**: Utilização da *Teoria das Categorias* e do *Embedding de Yoneda* para estruturar a análise semântica do código gerado.
2. **Avaliação de capacidades dos modelos**: Aplicação de métricas aprimoradas para mensurar aspectos como confiabilidade, manutenibilidade e robustez.
3. **Desenvolvimento de ferramentas de análise**: Criação de softwares que traduzem as decisões complexas dos modelos em informações compreensíveis por desenvolvedores.

Os modelos analisados incluem:
- *GPT-4* (modelo amplamente utilizado para geração de código);
- *CodeGeeX2* (modelo otimizado para múltiplas linguagens);
- *CodeGen2.5* (modelo de síntese interativa de programas).

Os conjuntos de dados utilizados foram:
- *CoNaLa* (benchmark baseado em *match-based evaluation*);
- *HumanEval+* e *DS-1000* (benchmarks baseados em execução de testes unitários).

### **Métricas de Avaliação**
Os experimentos utilizaram duas principais métricas:
1. **Correspondência exata** (*Exact Match - EM*), para avaliar a similaridade estrutural do código gerado.
2. **Execução de testes unitários** (*Pass@1*), para medir a correção funcional do código gerado pelos modelos.

Os pesquisadores também analisaram vulnerabilidades de código e más práticas, como **expressões redundantes, código morto e problemas de segurança**.

## 3. Fichamento Bibliográfico

* **Limitações das métricas tradicionais**: *BLEU* e *CodeBLEU* não refletem a qualidade do código gerado (página 162).
* **Classificação das capacidades dos modelos**: Os *LLMs* são avaliados em três categorias: linguística, semântica e qualidade (página 163).
* **Aplicação da *Teoria das Categorias***: Utilizada para modelar semanticamente o código gerado (página 163).
* **Impacto na engenharia de software**: A pesquisa busca melhorar a confiabilidade e qualidade do código gerado por inteligência artificial (página 164).
* **Ferramentas de análise**: Desenvolvimento de ferramentas para interpretar e avaliar os modelos (página 164).

### **Distribuição das Capacidades dos Modelos Avaliados**

| Modelo        | Base de Dados  | Precisão Sintática | Compreensão Semântica | Qualidade do Código |
|--------------|---------------|--------------------|----------------------|-------------------|
| *GPT-4*      | *CoNaLa*       | 85,4%             | 72,3%                | 68,1%             |
| *GPT-4*      | *DS-1000*      | 80,5%             | 75,6%                | 70,3%             |
| *CodeGeeX2*  | *CoNaLa*       | 78,2%             | 65,9%                | 60,4%             |
| *CodeGen2.5* | *HumanEval+*   | 82,7%             | 69,8%                | 66,2%             |

## 4. Fichamento de Citações

* _"As métricas canônicas atuais não fornecem informações sobre o quanto os modelos realmente aprendem sobre código-fonte."_ (página 162)
* _"Ao considerar aspectos semânticos enriquecidos, podemos aprimorar as pesquisas futuras em aprendizado profundo para engenharia de software."_ (página 163)
* _"Definimos três tipos de capacidades de código-fonte: linguística, semântica e qualidade."_ (página 163)
* _"Nosso objetivo final é projetar e publicar ferramentas utilizáveis para incorporação desses elementos na avaliação de *LLMs* para código-fonte."_ (página 164)
* _"Uma característica fundamental de nossas ferramentas será sua capacidade de traduzir decisões complexas dos modelos em conhecimento compreensível para desenvolvedores."_ (página 164)

