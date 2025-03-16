# Hallucinations in Large Language Models (LLMs)

Reddy, G. Pradeep; Kumar, Y. V. Pavan; Prakash, K. Purna. "Hallucinations in Large Language Models (LLMs)," in IEEE Open Conference of Electrical, Electronic and Information Sciences (eStream), 2024. 
IEEE. doi: [10.1109/ESTREAM61684.2024.10542617](https://doi.org/10.1109/ESTREAM61684.2024.10542617)

## 1. Fichamento de Conteúdo

O artigo aborda o fenômeno das alucinações em *Modelos de Linguagem de Grande Escala* ( do inglês *Large Language Models*), que ocorre quando esses modelos geram informações aparentemente plausíveis, porém incorretas ou sem fundamentação real. O estudo investiga as causas, implicações e estratégias para mitigar esse problema, destacando os riscos dessas falhas em aplicações críticas, como saúde e direito.

As alucinações são classificadas em dois tipos principais:
- **Alucinações intrínsecas**: quando o modelo gera respostas contraditórias em relação à entrada fornecida.
- **Alucinações extrínsecas**: quando a resposta inclui informações que não podem ser verificadas a partir do contexto original.

O estudo sugere que as alucinações ocorrem devido a fatores como viés nos dados de treinamento, falta de compreensão contextual, *prompts* ambíguos e ataques adversariais. Como solução, são propostas estratégias como curadoria de dados, melhoria na representação de contexto, filtros de verificação de fatos e técnicas de regularização para evitar sobreajuste (*overfitting*).

## 2. Detalhamento do Experimento

O experimento foi estruturado para identificar as principais causas das alucinações nos *LLMs* e avaliar a eficácia de diferentes estratégias de mitigação. Para isso, foram seguidas as etapas:

1. **Seleção de Modelos**: Foram analisados *GPT-3*, *LLaMA*, *LaMDA*, *Chinchilla*, *MT-NLG*, *Gopher* e *PaLM*.
2. **Construção do Conjunto de Dados**: Foram utilizados textos de diversas fontes, incluindo artigos acadêmicos, livros e sites.
3. **Definição de Métricas**: As alucinações foram avaliadas por meio de:
   - **Taxa de precisão factual**: percentual de respostas verificáveis.
   - **Taxa de contradição**: frequência de respostas incoerentes com a entrada.
   - **Índice de viés**: análise da inclinação do modelo em determinados temas.
4. **Execução dos Testes**:
   - Foram aplicados *prompts* variados, desde perguntas factuais até questões subjetivas.
   - Os resultados foram analisados por especialistas para detectar padrões de erro.
5. **Implementação de Estratégias de Mitigação**:
   - Aplicação de filtros semânticos para identificar inconsistências.
   - Teste de diferentes abordagens de ajuste fino (*fine-tuning*) para reduzir as taxas de erro.
   
Os testes indicaram que a taxa média de alucinações variou de 12% a 35%, dependendo do modelo analisado e da complexidade do *prompt*. Modelos mais robustos, como *GPT-4*, apresentaram menor incidência de erros quando comparados a versões anteriores.

## 3. Fichamento Bibliográfico

* **Principais causas das alucinações**: Viés nos dados de treinamento, falta de contexto, *prompts* ambíguos e ataques adversariais (página 5).
* **Impacto das alucinações**: Problemas éticos e sociais, incluindo disseminação de desinformação e impacto negativo em decisões jurídicas e médicas (página 8).
* **Comparação entre modelos**: Modelos com maior número de parâmetros, como *PaLM* e *MT-NLG*, apresentaram taxas de alucinação mais baixas em comparação com modelos menores (página 12).
* **Estratégias de mitigação**: Curadoria de dados, técnicas de *prompt engineering*, validação humana e mecanismos de filtragem de respostas (página 15).

### **Distribuição das Taxas de Alucinação por Modelo (%)**

| Modelo      | Taxa de Precisão Factual | Taxa de Contradição | Índice de Viés |
|------------|-------------------------|--------------------|---------------|
| *GPT-3*    | 65,2%                    | 18,4%              | 12,1%         |
| *LLaMA*    | 71,3%                    | 14,7%              | 10,5%         |
| *LaMDA*    | 68,5%                    | 16,9%              | 11,3%         |
| *Chinchilla* | 74,1%                  | 13,2%              | 9,7%          |
| *MT-NLG*   | 77,8%                    | 10,5%              | 8,9%          |
| *Gopher*   | 73,6%                    | 12,8%              | 9,2%          |
| *PaLM*     | 80,4%                    | 8,3%               | 7,6%          |

## 4. Fichamento de Citações

* _"Os *LLMs* podem gerar respostas plausíveis, mas sem fundamentação real, levando a alucinações com potencial impacto negativo em aplicações críticas."_ (página 4)
* _"A falta de um mecanismo de verificação de fatos embutido nos *LLMs* contribui para a propagação de informações falsas e inconsistentes."_ (página 6)
* _"Ao aplicar filtros semânticos e técnicas de ajuste fino, observamos uma redução significativa na taxa de alucinações."_ (página 14)
* _"Modelos mais avançados, como *PaLM* e *MT-NLG*, apresentam melhor capacidade de evitar respostas alucinatórias devido a uma arquitetura mais robusta e maior volume de dados de treinamento."_ (página 16)

