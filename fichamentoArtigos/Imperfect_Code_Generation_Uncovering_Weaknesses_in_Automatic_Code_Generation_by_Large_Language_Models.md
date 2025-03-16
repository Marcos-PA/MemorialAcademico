# Imperfect Code Generation: Uncovering Weaknesses in Automatic Code Generation by Large Language Models

Lian, Xiaoli; Wang, Shuaisong; Ma, Jieping; Tan, Xin; Liu, Fang; Shi, Lin; Zhang, Li; Gao, Cuiyun. "Imperfect Code Generation: Uncovering Weaknesses in Automatic Code Generation by Large Language Models," in 2024 
IEEE/ACM 46th International Conference on Software Engineering: Companion Proceedings (ICSE-Companion ’24), April 14–20, 2024, Lisbon, Portugal. ACM. doi: [10.1145/3639478.3643081](https://doi.org/10.1145/3639478.3643081)

## 1. Fichamento de Conteúdo

O artigo investiga as fragilidades na geração de código realizada por *Modelos de Linguagem de Grande Escala* ( do inglês *Large language Models*). O estudo avalia três modelos (*GPT-4*, *CodeGeeX2* e *CodeGen2.5*) utilizando três conjuntos de dados amplamente empregados na pesquisa: *CoNaLa*, *HumanEval+* e *DS-1000*. 

Os pesquisadores categorizam oito tipos principais de fraquezas na geração de código, incluindo falhas na interpretação de *prompts*, uso inadequado de *APIs* e redundância na geração de código. Como proposta de solução, o artigo sugere melhorias nos *benchmarks* e nos métodos de treinamento dos modelos para mitigar tais problemas e aprimorar a qualidade do código gerado.

## 2. Detalhamento do Experimento

Os experimentos foram conduzidos com um conjunto de modelos e bases de dados amplamente utilizados na área de geração automática de código. O estudo adotou dois tipos de avaliação:

1. **Avaliação baseada em correspondência** (*match-based evaluation*), utilizando a métrica *Exact Match (EM)*.
2. **Avaliação baseada em execução de testes unitários** (*unit-test execution-based evaluation*), mensurada pela métrica *Pass@1*.

### **Modelos Avaliados:**
- *GPT-4* (modelo da OpenAI amplamente utilizado em diversas aplicações de geração de código);
- *CodeGeeX2* (modelo multilíngue especializado em geração de código);
- *CodeGen2.5* (modelo de síntese de programas com abordagem interativa).

### **Bases de Dados Utilizadas:**
- *CoNaLa*: *benchmark* baseado em *match-based evaluation*.
- *HumanEval+* e *DS-1000*: *benchmarks* baseados em testes unitários.

Os pesquisadores selecionaram uma amostra representativa de casos de falha na geração de código e utilizaram análise temática para identificar as categorias de erros. O processo de anotação foi realizado por oito especialistas da área, incluindo um professor, um doutorando e seis pós-graduandos.

A metodologia seguiu as seguintes etapas:
1. Seleção aleatória de 339 amostras do conjunto *CoNaLa*, 115 de *HumanEval+* e 277 de *DS-1000*.
2. Identificação inicial de seis categorias de fraquezas em um estudo piloto.
3. Revisão colaborativa dos resultados para validação e inclusão de duas novas categorias de fraquezas.

## 3. Fichamento Bibliográfico

* **Categorias de fraquezas**: O estudo identifica oito principais problemas na geração de código por *LLMs*, incluindo *prompts* imprecisos, falhas semânticas e uso incorreto de *APIs* (página 3).
* **Impacto dos *prompts***: A qualidade do código gerado é diretamente influenciada pela clareza e precisão dos *prompts*, sendo que *prompts* excessivamente complexos aumentam as taxas de erro (página 5).
* **Uso incorreto de *APIs***: Erros comuns incluem parâmetros incorretos ou chamadas para *APIs* inexistentes, impactando negativamente a funcionalidade do código (página 6).
* **Sugestões de melhoria**: O estudo propõe *benchmarks* mais sofisticados e estratégias avançadas de treinamento para reduzir erros na geração de código (página 8).

### **Distribuição dos Tipos de Fraquezas por Modelo (%)**

| Modelo        | Base de Dados | *Prompts* Imprecisos | *Prompts* Complexos | Viés de Respostas | Semântica Perdida | Erros de *API* | Falha de Conhecimento | Código Excessivo | Código Redundante |
|--------------|--------------|----------------------|----------------------|-------------------|------------------|---------------|------------------|---------------|----------------|
| *GPT-4*     | *CoNaLa*      | 27,14                | 0,88                 | 43,66             | 8,85             | 0,59          | 1,18             | 5,60          | 0,00          |
| *GPT-4*     | *DS-1000*     | 8,47                 | 7,41                 | 0,00              | 55,56            | 1,59          | 0,00             | 1,59          | 0,00          |
| *CodeGeeX2* | *CoNaLa*      | 27,14                | 1,18                 | 32,15             | 39,82            | 2,36          | 2,65             | 10,62         | 4,13          |
| *CodeGen2.5*| *CoNaLa*      | 27,43                | 0,88                 | 23,01             | 54,28            | 2,36          | 2,06             | 8,55          | 0,00          |

## 4. Fichamento de Citações

* _"Apesar de alcançarem desempenho de última geração, os *LLMs* ainda geram código com fraquezas significativas que precisam ser abordadas."_ (página 2)
* _"Nosso estudo identifica oito categorias distintas de fraquezas na geração de código e destaca sua prevalência em múltiplos *benchmarks*."_ (página 4)
* _"*Prompts* imprecisos levam a interpretações errôneas, tornando quase impossível para os *LLMs* gerarem código correto."_ (página 5)
* _"Propomos o refinamento dos *benchmarks* para incluir soluções diversificadas de *API* e melhorar a representação semântica dos *prompts* para aumentar a precisão do código gerado."_ (página 8)
* _"A redundância na geração de código permanece um problema crítico que exige estratégias específicas para mitigação."_ (página 8)



