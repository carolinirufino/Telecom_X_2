# 📊 Análise de Evasão de Clientes (Churn Prediction)

Este projeto tem como objetivo identificar os principais fatores que influenciam a evasão de clientes em uma empresa de telecomunicações, utilizando técnicas de aprendizado de máquina para construir modelos preditivos confiáveis. A proposta vai além da previsão: buscamos entender o "porquê" da saída e propor estratégias práticas de retenção.

---

## 💡 Objetivos

- Analisar o perfil dos clientes e identificar padrões de evasão.
- Aplicar técnicas de Machine Learning para prever o churn.
- Comparar o desempenho entre modelos com e sem normalização.
- Utilizar balanceamento de classes (SMOTE) para melhorar a equidade dos modelos.
- Gerar insights claros e aplicáveis para estratégias de retenção.

---

## 🧠 Modelos Utilizados

Foram testados dois modelos principais:

### 1. **Regressão Logística com SMOTE**
- Requer normalização dos dados.
- Bom para interpretar a influência de cada variável (coeficientes).
- Destaque para variáveis como `Encargos_Mensais`, `Encargos_Totais` e `Tempo_Servico`.

### 2. **Random Forest com SMOTE**
- Não exige normalização.
- Indicado para captar relações complexas entre variáveis.
- Destaque para `Tempo_Servico`, `Encargos_Totais`, e `Contrato_Conta`.

---

## 🔎 Principais Insights

### 🔥 Fatores que aumentam a evasão:
- Altos **encargos mensais** e **totais**.
- Clientes com **contrato mensal**.
- Usuários de **internet por fibra óptica**, que apesar de mais veloz, podem ter maiores custos e expectativas.
- Baixo tempo de serviço com a empresa.

### ❄️ Fatores que reduzem a evasão:
- Clientes **antigos**, com maior tempo de vínculo.
- Usuários com **contrato bienal**.
- Clientes que **possuem dependentes ou parceiro** no cadastro — sinal de envolvimento mais profundo com o serviço.

---

## 🛠️ Técnicas Aplicadas

- **Pré-processamento** de dados (encoding, normalização).
- **Balanceamento de classes com SMOTE**.
- **GridSearchCV** para ajuste de hiperparâmetros.
- **Avaliação com métricas clássicas**: Acurácia, Precisão, Recall, F1-score, e Matriz de Confusão.
- **Análise interpretativa dos coeficientes e importâncias das variáveis**.

---

## 📈 Métricas de Avaliação

| Modelo                       | Acurácia | Precisão | Recall | F1-score |
|-----------------------------|----------|----------|--------|----------|
| Regressão Logística (SMOTE) | 0.7611   | 0.5287   | 0.6578 | 0.5862   |
| Random Forest (SMOTE)       | 0.7652   | 0.5375   | 0.6257 | 0.5783   |

Ambos os modelos apresentaram desempenho semelhante. A regressão logística se destacou no recall, enquanto a random forest apresentou maior estabilidade geral.

---

## 🎯 Conclusão

A análise demonstrou que a evasão não acontece ao acaso — ela responde a padrões claros de comportamento, relacionamento e percepção de valor. Modelos preditivos, quando bem interpretados, tornam-se aliados estratégicos na construção de ações mais humanas, personalizadas e eficazes.

> *“Mais do que prever a saída, este projeto busca compreender o silêncio antes da despedida — e transformá-lo em oportunidade de reconexão.”*

---

## 💻 Como Usar

- Clone o repositório
- Abra o notebook .ipynb no Jupyter ou Google Colab
- Execute as células para seguir a análise passo a passo

## 🧾 Requisitos

- Python 3.x
- pandas, numpy, matplotlib, seaborn
- scikit-learn, imblearn

---

## 🧠 Próximos Passos

- Testar novos modelos (XGBoost, LightGBM).
- Explorar variáveis temporais e de engajamento mais profundo.
- Integrar os resultados a uma dashboard interativa.

---

## ✍️ Autoria

**Carolini Rufino**  
Estudante de Data Science | Bacharel em Administração de Empresas

📧 carolinirufino@gmail.com

🔗 [LinkedIn](https://www.linkedin.com/in/carolinirufino)

---
