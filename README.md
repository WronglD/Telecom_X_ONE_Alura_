# Telecom_X_ONE_Alura
# 📊 Projeto de Previsão de Churn - Telecom X (Parte 2)  

---

## 1. Objetivo Geral  
O foco deste trabalho foi construir um modelo de **Machine Learning** capaz de prever a evasão de clientes (churn) da empresa fictícia **Telecom X**.  
Além de desenvolver um classificador eficiente, buscou-se também entender quais aspectos demográficos e relacionados ao uso dos serviços mais impactam a decisão de cancelamento, de forma a apoiar estratégias de negócio.  

---

## 2. Estrutura do Projeto e Ferramentas Utilizadas  
O desenvolvimento foi realizado em um notebook Jupyter (`.ipynb`) com **Python** e as seguintes bibliotecas principais:  

- **Pandas:** limpeza, manipulação e preparação dos dados.  
- **Scikit-learn:** construção, treinamento e avaliação dos modelos, além do escalonamento das variáveis.  
- **Matplotlib / Seaborn (opcional):** visualização exploratória dos dados.  

📂 Organização do repositório:  
- `README.md`: documentação detalhada do projeto.  
- `analise_churn_parte2.ipynb`: notebook com código e análises.  
- `dados_tratados.csv`: dataset final, já limpo e pronto para a modelagem.  

---

## 3. Modelos Testados e Resultados  
Foram comparados dois algoritmos de classificação: **Regressão Logística** e **Random Forest**.  

O modelo escolhido foi a **Regressão Logística**, que apresentou melhor desempenho no critério mais relevante para o negócio: identificar corretamente os clientes com risco real de evasão.  

📊 Comparativo de métricas:  

| Métrica                | Regressão Logística | Random Forest |
|-------------------------|----------------------|---------------|
| **Acurácia Geral**      | 79.74%              | 77.75%        |
| **Recall (Churn = 1)**  | 54%                 | 46%           |
| **Precisão (Churn = 1)**| 64%                 | 61%           |

> O **recall** foi usado como métrica decisiva, pois mede a capacidade do modelo de identificar os clientes que realmente irão cancelar — permitindo ações preventivas da empresa.  

---

## 4. Insights da Análise  
A interpretação dos coeficientes da **Regressão Logística** revelou os principais fatores que influenciam o churn:  

🔺 **Fatores de Risco (aumentam a chance de evasão)**  
- **Tipo de Internet:** uso de Fibra Óptica é o maior indicador de risco.  
- **Forma de Pagamento:** clientes que utilizam **Cheque Eletrônico** têm maior propensão a cancelar.  
- **Fatura Digital:** adesão ao *Paperless Billing* também se relaciona a uma maior taxa de churn.  

🔻 **Fatores de Retenção (reduzem a chance de evasão)**  
- **Tipo de Contrato:** planos de **1 ou 2 anos** são o fator mais protetor contra cancelamentos.  
- **Serviços Extras:** contratação de **Suporte Técnico** e **Segurança Online** está fortemente associada à fidelização.  

---

## 5. Recomendações Estratégicas  
Com base nos resultados, são sugeridas as seguintes ações:  

1. **Fidelização via Contrato:** campanhas de marketing com descontos ou benefícios para incentivar clientes de planos mensais a aderirem a contratos mais longos (1–2 anos).  
2. **Avaliação do Serviço de Fibra:** conduzir uma investigação detalhada (como pesquisas de satisfação) com usuários de Fibra Óptica para entender os motivos da alta taxa de evasão — preço, qualidade ou concorrência.  
3. **Agregação de Valor:** promover pacotes que incluam **Suporte Técnico** e **Segurança Online** como diferenciais, já que mostraram impacto positivo na retenção.  

---

## 6. Como Executar o Projeto  
1. Clone este repositório na sua máquina.  
2. Verifique se possui o **Python** e as bibliotecas necessárias instaladas (`pandas`, `scikit-learn`, etc.).  
3. Abra o notebook `analise_churn_parte2.ipynb` em um ambiente como **Jupyter Notebook** ou **Google Colab**.  
4. Caso use o Google Colab, faça o upload do arquivo `dados_tratados.csv` para o ambiente.  
5. Execute as células do notebook na ordem indicada.

---
   
## 📧 Contato  
- **Responsável:** Alisson Matheus  
- **E-mail:** alisson.ssilva@ufpe.br  

---

ℹ️ Este projeto foi elaborado com propósito **educacional** no âmbito do **Programa Alura ONE**.
