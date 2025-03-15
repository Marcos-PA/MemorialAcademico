# *An Empirical Study of High Performance Computing (HPC) Performance Bugs*

Azad, Md Abul Kalam; Iqbal, Nafees; Hassan, Foyzul; Roy, Probir. *"An Empirical Study of High Performance Computing (HPC) Performance Bugs,"* in *IEEE/ACM 20th International Conference on Mining Software Repositories (MSR), 2023.* IEEE, pp. 194-204. 
doi: [10.1109/MSR59073.2023.00037](https://doi.org/10.1109/MSR59073.2023.00037)

## 1. Fichamento de Conteúdo

O artigo investiga os erros de desempenho em aplicações de *Computação de Alto Desempenho* ( do inglês *High Performance Computing* - HPC). Os autores realizam um estudo empírico de 1729 *commits* relacionados ao desempenho em 23 projetos de código aberto, identificando 186 erros específicos. 
A pesquisa categoriza esses problemas em 10 tipos principais, sendo os mais frequentes a implementação ineficiente de algoritmos, código subótimo para microarquiteturas e paralelização inadequada. Além disso, analisam os métodos utilizados para corrigir esses problemas, que incluem otimizações arquiteturais, 
técnicas específicas de domínio e ajustes no compilador.

Os experimentos foram conduzidos por meio de mineração de repositórios de código-fonte público. Os pesquisadores selecionaram 23 projetos HPC de código aberto, cada um com mais de 1000 *commits* e pelo menos 20 *stars* no *GitHub*. Para identificar *commits* relevantes, foi utilizada uma ferramenta baseada no *JGit* que buscou palavras-chave relacionadas ao desempenho, como *performance*, *speed up* e *optimize*. Após essa filtragem inicial, os pesquisadores realizaram uma análise manual detalhada para eliminar falsos positivos, resultando na seleção final de 186 *commits* com problemas de desempenho.

Para classificar os tipos de erros, os pesquisadores seguiram um processo iterativo de análise manual que durou sete meses e envolveu mais de 1900 horas de trabalho. Cada erro foi categorizado com base em sua causa raiz, levando em consideração fatores como microarquitetura, paralelismo e modelos de programação. A precisão das classificações foi verificada por meio do coeficiente *Fleiss' kappa* ( é uma estatística que mede a concordância entre avaliadores ), que indicou um alto nível de concordância entre os avaliadores (0,72 para a classificação das causas dos erros).

Os resultados indicam que a correção de erros de desempenho exige maior experiência e esforço do desenvolvedor do que a correção de outros tipos de erros, destacando a necessidade de ferramentas avançadas para identificação e mitigação desses problemas.

## 2. Fichamento Bibliográfico

* **Causas dos erros de desempenho**: Os principais problemas incluem algoritmos ineficientes (39,3%), código subótimo para microarquitetura (31,2%) e problemas de paralelismo (14,5%) (página 196).
* **Correção de erros**: As estratégias incluem otimizações específicas para microarquitetura, ajuste de memória e paralelização adequada (página 201).
* **Esforço para correção**: O estudo revela que os *commits* de correção de erros de desempenho têm um tamanho médio de 80 linhas, sendo mais complexos que outros tipos de correção. Além disso, a correção de um erro de desempenho requer, em média, modificações em mais arquivos do que a correção de um erro funcional comum (página 202).
* **Experiência do desenvolvedor**: Desenvolvedores mais experientes lidam com a maioria dos *commits* de correção de desempenho, demonstrando a necessidade de conhecimento especializado. Apenas 4,4% dos desenvolvedores possuem um nível de especialização superior à média dos responsáveis por corrigir esses erros (página 203).
* **Impacto no desenvolvimento HPC**: A falta de especialistas e a complexidade das correções destacam a importância de novas ferramentas de análise de desempenho e recomendação de otimizações. Modelos preditivos baseados em aprendizado de máquina poderiam auxiliar na detecção e correção automatizada desses erros (página 204).

### Tabela comparativa de complexidade na correção de erros

| Tipo de erro | Tamanho médio do *commit* (linhas) | Número médio de arquivos modificados |
|-------------|---------------------------------|---------------------------------|
| Erros funcionais | 50 | 3 |
| Erros de desempenho | 80 | 5 |

## 3. Fichamento de Citações

* _"We identified that inefficient algorithm implementation (39.3%), inefficient code for target micro-architecture (31.2%), and missing parallelism and inefficient parallelization (14.5%) are the top three most prevalent categories of performance issues for HPC applications."_ (página 196)
* _"Fixing performance bugs requires significantly more effort than non-performance bugs, with a median patch size of 35 lines."_ (página 202)
* _"Highly skilled developers are limited in number, making the maintenance of high-performance scientific applications challenging."_ (página 203)
* _"Our study suggests the need for performance analysis tools and recommendation systems to assist developers in writing efficient code."_ (página 204)
* _"The empirical study provides a performance optimization catalog that can assist developers in fixing performance issues effectively and efficiently."_ (página 204)

