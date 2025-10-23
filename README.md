# 📝 Redmine Interativa – Projeto Previsão de Futebol com IA Claude no Databricks

![Databricks](https://img.shields.io/badge/Databricks-Workspace-blue)
![Python](https://img.shields.io/badge/python-3.9+-blue)
![Colab](https://img.shields.io/badge/Colab-Open-orange)
![License](https://img.shields.io/badge/license-MIT-green)

---

## ✅ Status Geral
O pipeline foi **totalmente executado**, com todas as camadas concluídas e resultados registrados.

---

## 1️⃣ Bronze – Ingestão de Dados

**Objetivo:** Coletar e armazenar dados brutos no DBFS.  

**Tarefas Concluídas:**
- [x] Identificação e catalogação de fontes de dados (APIs, CSVs, dados abertos)  
- [x] Notebooks de ingestão criados e executados  
- [x] Dados brutos validados  
- [x] Tabelas Delta Bronze criadas  
- [x] Esquemas documentados  

**Notebook:** [01_Bronze_Ingestao](https://colab.research.google.com/github/projetosdatabricksfree-png/projeto-previsao-futebol-claude/blob/main/notebooks/01_Bronze_Ingestao.ipynb)

---

## 2️⃣ Silver – Processamento de Dados

**Objetivo:** Limpeza, transformação e padronização dos dados.  

**Tarefas Concluídas:**
- [x] Remoção de inconsistências e valores nulos  
- [x] Normalização de formatos (datas, nomes, estatísticas)  
- [x] Transformação de variáveis para análise  
- [x] Atualização das tabelas Delta Silver  
- [x] Rastreabilidade de alterações garantida  

**Notebook:** [02_Silver_Processamento](https://colab.research.google.com/github/projetosdatabricksfree-png/projeto-previsao-futebol-claude/blob/main/notebooks/02_Silver_Processamento.ipynb)

---

## 3️⃣ Gold – Engenharia de Atributos

**Objetivo:** Criar features e métricas relevantes para os modelos.  

**Tarefas Concluídas:**
- [x] Criação de métricas históricas de times e jogadores  
- [x] Features como streaks de vitórias, média de gols, desempenho casa/fora  
- [x] Análise exploratória de dados (EDA)  
- [x] Atualização das tabelas Delta Gold  
- [x] Documentação das features  

**Notebook:** [03_Gold_Eng_Atributos](https://colab.research.google.com/github/projetosdatabricksfree-png/projeto-previsao-futebol-claude/blob/main/notebooks/03_Gold_Eng_Atributos.ipynb)

---

## 4️⃣ Diamond – Treinamento de Modelos

**Objetivo:** Treinar e avaliar modelos usando dados Gold.  

**Tarefas Concluídas:**
- [x] Seleção de algoritmos (Random Forest, Logistic Regression)  
- [x] Treinamento com validação cruzada  
- [x] Avaliação de performance: Accuracy, F1-score, AUC  
- [x] Registro de modelos no MLflow  
- [x] Documentação de hiperparâmetros e métricas  

**Notebook:** [04_Diamond_Treinamento](https://colab.research.google.com/github/projetosdatabricksfree-png/projeto-previsao-futebol-claude/blob/main/notebooks/04_Diamond_Treinamento.ipynb)

---

## 5️⃣ Diamond – Inferência e Previsão

**Objetivo:** Aplicar modelos e gerar previsões e insights automáticos.  

**Tarefas Concluídas:**
- [x] Execução do pipeline de inferência com dados atualizados  
- [x] Geração de relatórios e dashboards  
- [x] Integração com IA Claude para insights automáticos  
- [x] Atualização da tabela Delta de inferência  
- [x] Registro de erros, alertas e métricas da execução final  

**Notebook:** [05_Diamond_Inferencia](https://colab.research.google.com/github/projetosdatabricksfree-png/projeto-previsao-futebol-claude/blob/main/notebooks/05_Diamond_Inferencia.ipynb)

---

## 📊 Resultados da Execução Final – 22/10/2025

| Item | Valor |
|------|-------|
| Modelo Estatístico (Logistic Regression) | ✅ `modelo_lr` |
| Modelo Tático (RandomForest) | ✅ `modelo_rf` |
| Meta-Modelo (Logistic Regression) | ✅ `modelo_final` |
| Mapeamento de Labels | ✅ `df_labels_map` – 3 registros |
| Acurácia do Modelo Geral | ✅ `acc_geral` – 43.64% |
| Acurácia do Modelo LR | ✅ `acc_lr` – 49.09% |
| Acurácia do Modelo RF | ✅ `acc_rf` – 43.64% |
| Acurácia do Meta-Modelo | ✅ `acuracia` – 56.36% |
| DataFrame de Treino | ✅ `df_treino` – 218 registros |
| DataFrame de Teste | ✅ `df_teste` – 55 registros |

---

## 📊 Métricas de Execução Consolidada

| Data Execução | Camada | Status | Métricas Principais | Observações |
|---------------|--------|--------|-------------------|-------------|
| 22/10/2025 | Bronze | ✅ Concluído | - | Dados brutos coletados e Delta Bronze criado |
| 22/10/2025 | Silver | ✅ Concluído | - | Delta Silver atualizado |
| 22/10/2025 | Gold | ✅ Concluído | - | Delta Gold atualizado com features |
| 22/10/2025 | Diamond Treinamento | ✅ Concluído | Modelo LR: 49.09% <br>Modelo RF: 43.64% <br>Modelo Geral: 43.64% <br>Meta-Modelo: 56.36% | Modelos registrados no MLflow |
| 22/10/2025 | Diamond Inferência | ✅ Concluído | Treino: 218 registros <br>Teste: 55 registros <br>Previsões geradas e insights Claude | Pipeline finalizado com sucesso |

---

## 🖇 Referências

- [Databricks Documentation](https://docs.databricks.com/)  
- [Delta Lake](https://delta.io/)  
- [MLflow](https://mlflow.org/)  
- [Claude AI](https://www.anthropic.com/)  

---

## 🔖 Licença

Este projeto está licenciado sob a **MIT License**.
