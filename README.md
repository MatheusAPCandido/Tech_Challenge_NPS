# Tech_Challenge_NPS
# POSTECH_AI_SCIENTIST_DESAFIO


## Estrutura do repositório:
📁 AI_Scientist
- Código da Análise Exploratória
📁Apresentacao
- PDF Slides de apresentação
- Video Executivo
📁 Base_de_dados 
Excel banco de dados
📁 Documentos
Respostas Requisitos:
- Análise Exploratória de Dados
- Definição de Target
- NPS

# Tech Challenge: Previsão de Risco de Detratação (NPS) no E-commerce

Este projeto faz parte do Tech Challenge da Pós-Graduação em Data Science, com o objetivo de analisar e prever o comportamento de clientes insatisfeitos (**Detratores**) para apoiar tomadas de decisão estratégicas e preventivas.

## 🎯 Objetivo do Projeto

O objetivo principal é transformar dados operacionais (logística, suporte e financeiro) em inteligência de negócio. O foco está em identificar quais falhas nos processos de e-commerce levam um cliente a se tornar um detrator (notas de 0 a 6 no NPS).

A análise busca responder:
1. Quais são os principais "vilões operacionais" que destroem a satisfação do cliente?
2. É possível prever o risco de detratação antes mesmo do cliente responder à pesquisa?
3. Quais ações práticas o time de Customer Experience (CX) pode tomar para mitigar danos?

## 📊 Descrição da Base de Dados

A base de dados utilizada é a `desafio_nps_fase_1.csv`, que contém **2.500 registros** de transações de e-commerce com 19 variáveis, incluindo:

* **Perfil do Cliente:** Idade, região e tempo de relacionamento (tenure).
* **Dados Logísticos:** Tempo de entrega, dias de atraso e tentativas de entrega.
* **Dados de Atendimento:** Número de contatos com suporte, tempo de resolução e contagem de reclamações.
* **Dados Financeiros:** Valor do pedido, frete e parcelamento.
* **Target (NPS):** Pontuação de 0 a 10 atribuída pelo cliente.

### Distribuição do Target:
Nesta base específica, observou-se um cenário crítico com **74,04% de Detratores**, tornando a análise de causa raiz ainda mais vital para a sobrevivência do negócio.

## 🧠 Metodologia Utilizada

O projeto seguiu as seguintes etapas de Ciência de Dados:

1.  **Análise Exploratória de Dados (EDA):** Identificação de distribuições, detecção de outliers e análise de correlação entre variáveis operacionais e a nota de NPS.
2.  **Definição do Alvo (Target):** Criação de uma variável binária (`is_detrator`) onde notas ≤ 6 foram classificadas como 1 (risco alto) e notas > 6 como 0.
3.  **Investigação de Causa Raiz:** Comparação de médias entre os grupos para identificar "Gaps" de performance (ex: o atraso logístico é 111% superior no grupo de detratores).
4.  **Storytelling e Insights:** Tradução dos dados técnicos em recomendações práticas, focadas na redução do esforço do cliente e gestão proativa de atrasos.

## 🚀 Como Reproduzir os Resultados

Para executar este projeto localmente, siga os passos abaixo:

### Pré-requisitos
* Python 3.8+
* Bibliotecas: `pandas`, `numpy`, `matplotlib`, `seaborn`

### Passo a Passo
1.  Clone este repositório:
    ```bash
    git clone [https://github.com/MatheusAPCandido/Tech_Challenge_NPS.git](gh repo clone MatheusAPCandido/Tech_Challenge_NPS)
    ```
2.  Instale as dependências:
    ```bash
    pip install pandas numpy matplotlib seaborn
    ```
3.  Execute o script de análise ou o Jupyter Notebook:
    ```python
    import pandas as pd
    # Carregar a base
    df = pd.read_csv('Base de dados Desafio Tecnológico/desafio_nps_fase_1.csv')
    # Rodar análises
    ```

---
**Autor:** Vangelo Moreira de Araújo Filho / Matheus Augusto de Paiva Candido 
*Estudantse de Data Science - POSTECH*
