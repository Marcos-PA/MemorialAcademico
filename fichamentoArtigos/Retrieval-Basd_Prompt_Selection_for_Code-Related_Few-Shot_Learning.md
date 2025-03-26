# *Retrieval-Based Prompt Selection for Code-Related Few-Shot Learning*

Noor Nashid; Mifta Sintaha; Ali Mesbah. *"Retrieval-Based Prompt Selection for Code-Related Few-Shot Learning"*, in *45th International Conference on Software Engineering (ICSE), 2023.* IEEE. doi: [10.1109/ICSE48619.2023.00205](https://doi.org/10.1109/ICSE48619.2023.00205)

## 1. Fichamento de Conteúdo

O artigo investiga a criação de *prompts* eficazes para aprendizado de poucos exemplos ( do inglés *few-shot learning*) em tarefas relacionadas a código-fonte. Os autores propõem uma técnica de seleção automática de demonstrações de código, baseada em análise de embeddings ou frequência, chamada **CEDAR**.

A técnica foi aplicada em duas linguagens de programação (tipadas e dinamicamente tipadas) e duas tarefas: **geração de asserções de teste** e **reparo de código**. O desempenho de CEDAR foi comparado a modelos específicos para tarefas e modelos ajustados (*fine-tuned*).

Os resultados experimentais mostram que a abordagem proposta melhora a precisão das tarefas sem a necessidade de treinamento específico para cada tarefa ou linguagem. CEDAR obteve precisão de 76% na geração de asserções de teste e 52% no reparo de código, superando modelos de estado da arte.

## 2. Fichamento Bibliográfico

* **Aprendizado de poucos exemplos em tarefas de código**: O artigo propõe um método para selecionar exemplos relevantes automaticamente e construir *prompts* eficazes (página 2).
* **Modelo CEDAR**: Técnica de recuperação baseada em embeddings ou frequência para selecionar exemplos relevantes para *few-shot learning* (página 4).
* **Geração de asserções de teste**: Utilização de *few-shot learning* para gerar asserções automaticamente em testes unitários (página 6).
* **Reparo de código**: Aplicação da técnica para corrigir erros de código identificados por analisadores estáticos (*linters*) (página 7).
* **Comparação com modelos *fine-tuned***: CEDAR supera modelos ajustados e específicos para tarefas sem necessidade de treinamento extenso (página 10).
* **Resultados experimentais**: A seleção de demonstrações baseadas em embeddings foi mais eficaz do que métodos aleatórios ou *zero-shot* (página 12).

### Tabela comparativa de precisão das técnicas

| Método | Geração de Asserções | Reparo de Código |
|--------|----------------------|-----------------|
| Modelos específicos | 17.66% | 7.90% |
| Modelos *fine-tuned* | 68.93% | 49.30% |
| CEDAR | **76.55%** | **51.72%** |

* **Sugestões para pesquisas futuras**: Aplicação da abordagem a mais tarefas e integração com ferramentas de desenvolvimento como plugins de IDE (página 14).

## 3. Fichamento de Citações

* _"Selecting relevant examples using retrieval-based techniques significantly improves few-shot learning for code-related tasks."_ (página 5)
* _"Our approach outperforms fine-tuned models without requiring task-specific training data."_ (página 10)
* _"CEDAR achieves state-of-the-art results in both assertion generation and program repair tasks with minimal examples."_ (página 12)
* _"Future research should explore expanding CEDAR’s applicability to a wider range of programming tasks."_ (página 14)

