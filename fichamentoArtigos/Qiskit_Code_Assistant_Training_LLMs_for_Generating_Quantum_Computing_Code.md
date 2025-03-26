# *Qiskit Code Assistant: Training *LLMs* for Generating *Quantum Computing Code*

Nicolas Dupuis; Luca Buratti; Sanjay Vishwakarma; Aitana Viudes Forrat; David Kremer; Ismael Faro; Ruchir Puri; Juan Cruz-Benito. *"Qiskit Code Assistant: Training *LLMs* for Generating *Quantum Computing Code*,"* in *IEEE *LLM* Aided Design Workshop (*LAD*), 2024.* *IEEE*. doi: [10.1109/LAD62341.2024.10691762](https://doi.org/10.1109/LAD62341.2024.10691762)

## 1. Fichamento de Conteúdo

O artigo apresenta o **Qiskit Code Assistant**, um modelo de linguagem treinado para auxiliar no desenvolvimento de código quântico com o **Qiskit *SDK***. Os autores exploram os desafios da geração de código quântico e propõem uma abordagem especializada para treinar *Large Language Models (*LLMs*)* com dados específicos da área.

Os principais desafios abordados incluem:
- A necessidade de conhecimento especializado em computação quântica;
- A escassez de dados de código quântico disponíveis;
- A rápida evolução do campo e das bibliotecas relacionadas.

Para superar esses desafios, os autores treinaram o modelo **Granite-20B-Code-QK**, uma versão do modelo *Granite-20B-Code* adaptada ao contexto da computação quântica. O treinamento envolveu dados coletados do *GitHub*, incluindo scripts *Python* e *Jupyter Notebooks* contendo código do *Qiskit*.

Os resultados mostraram que o modelo especializado superou outras abordagens em tarefas específicas de código quântico, avaliadas por meio do **Qiskit *HumanEval* (*QHE*)**, um novo *benchmark* desenvolvido pelos autores. O modelo atingiu **46,53% de precisão** no *QHE*, superando modelos genéricos como **DeepSeek-Coder-33B** e **StarCoder2-15B**.

## 2. Fichamento Bibliográfico

* **Desafios na geração de código quântico**: Necessidade de conhecimento especializado e dados limitados dificultam o uso de *LLMs* genéricos para computação quântica (página 3).
* **Treinamento do modelo *Granite-20B-Code-QK***: Uso de um modelo base da família *Granite* aprimorado com dados específicos do *Qiskit* (página 5).
* **Coleta e processamento dos dados**: Repositórios *GitHub* foram filtrados para incluir apenas código atualizado e relevante (página 6).
* **Benchmark *Qiskit HumanEval* (*QHE*)**: Desenvolvimento de um conjunto de testes baseado no *Qiskit* para avaliar modelos de código quântico (página 8).
* **Comparação de desempenho**: O modelo *Granite-20B-Code-QK* superou modelos de código genéricos, atingindo melhor precisão no *benchmark QHE* (página 10).
* **Aplicação futura do modelo**: Integração com *IDEs* e ferramentas de desenvolvimento para auxiliar programadores quânticos (página 12).

### Tabela comparativa de precisão no *QHE*

| Modelo | Precisão no *QHE* |
|--------|----------------|
| *CODELLAMA-34B-PYTHON-HF* | 26.73% |
| *DEEPSEEK-CODER-33B-BASE* | 39.60% |
| *DEEPSEEK-CODER-33B-INSTRUCT* | 35.64% |
| *STARCODER2-15B* | 37.62% |
| *GRANITE-20B-CODE* | 20.79% |
| **GRANITE-20B-CODE-QK** | **46.53%** |

* **Sugestões para pesquisas futuras**: Atualização contínua dos modelos para acompanhar a evolução do *Qiskit* e expansão para outras linguagens de computação quântica (página 14).

## 3. Fichamento de Citações

* _"Training specialized *LLMs* for quantum computing code generation can significantly improve accuracy over generic models."_ (página 4)
* _"Our *Qiskit HumanEval* benchmark provides a structured approach to evaluate code generation in quantum computing."_ (página 8)
* _"The *Granite-20B-Code-QK* model outperforms state-of-the-art code *LLMs* in *QHE*, demonstrating the benefits of domain-specific training."_ (página 10)
* _"Future work includes integrating our model into development environments to streamline quantum programming workflows."_ (página 12)

