# BEM LUNOS
---
**Ordem do Café Sagrado**- "Sem cafeína não há vitória".
---
**Integrantes:** Gisela Ceresér Kassick, Giovani M. Nagano e Rebeka L. Batichotti  
**Instituição:** Ilum – Escola de Ciência – CNPEM  
**Disciplina:** Prática em Ciência de Dados  
**Professores orientadores:** Daniel R. Cassar  

---

**BEM LUNOS** é um projeto interdisciplinar que aplica **técnicas de aprendizado de máquina** e **ciência de dados** para compreender e prever o desempenho estudantil com base em fatores sociais, psicológicos e comportamentais.  
O **dataset Student Performance Factors**, disponível no **Kaggle**, reúne informações sobre estudantes, incluindo hábitos de estudo, tempo de sono, atividades extracurriculares e suporte familiar, com o objetivo de compreender como esses elementos influenciam o desempenho acadêmico. A análise desse conjunto de dados permite identificar **padrões** que auxiliam na formulação de estratégias mais eficazes para promover o aprendizado e o sucesso escolar.

A partir disso, diferentes modelos de aprendizado de máquina são comparados para identificar quais algoritmos apresentam **maior precisão preditiva** e **melhor interpretabilidade**, contribuindo para uma compreensão mais ampla dos determinantes do sucesso escolar.  

---

## Sumário

- [Sobre o projeto](#sobre-o-projeto)  
- [Como Executar](#como-executar)  
- [Especificações Técnicas](#especificações-técnicas)  
- [Referências](#referências)  
- [Professores orientadores](#professor-orientador)  
- [Contribuições da Equipe](#contribuições-da-equipe)  

---

## Sobre o projeto

O **desempenho estudantil** é um dos principais indicadores de qualidade educacional e está intimamente relacionado a variáveis socioeconômicas, cognitivas e emocionais.  
O **BEM LUNOS** visa **analisar esses fatores** e **prever as notas finais** de estudantes a partir de modelos supervisionados de regressão, promovendo uma visão quantitativa e interpretável do processo de aprendizagem.

Baseado no dataset *Student Performance Factors*, o projeto inclui todas as etapas de um pipeline de ciência de dados:
- **Pré-processamento:** limpeza e normalização dos dados, tratamento de valores ausentes e codificação de variáveis categóricas.  
- **Análise exploratória (EDA):** estudo de correlações e distribuição das variáveis.  
- **Modelagem preditiva:** implementação e comparação de algoritmos de aprendizado de máquina.  
- **Avaliação:** cálculo de métricas de desempenho (MAE, RMSE, R²).  

Além da previsão numérica, o modelo auxilia na **identificação dos fatores mais relevantes** para o rendimento acadêmico, o que pode subsidiar **políticas educacionais baseadas em evidências**.

---

## Como Executar

### Requisitos
- Python 3  
- Bibliotecas: `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`, `optuna` e `SHAP` 
- Jupyter Notebook ou VSCode com suporte a Python  

### Instalação
```bash
git clone https://github.com/GiselaCK/bem_lunos.git
cd bem_lunos
pip install numpy pandas scikit-learn matplotlib seaborn optuna SHAP
```
---

# Especificações Técnicas

## Linguagens e Tecnologias

- **Python** – Análise de dados e modelagem preditiva  
- **Scikit-learn** – Implementação dos modelos de aprendizado de máquina  
- **Matplotlib / Seaborn** – Visualização de dados e correlações  
- **Jupyter Notebook** – Ambiente interativo de execução e análise
- **Optuna** - Otimização de hiperparâmetros
- **SHAP** - Análise dos modelos

---

## Modelos Utilizados

O projeto implementa e compara **cinco abordagens principais**:

### 1. K-Nearest Neighbors (KNN)
- Método baseado na similaridade entre amostras. A previsão é feita com base nas k observações mais próximas no espaço de características. É simples e eficiente para dados com relações locais bem definidas.

### 2. Random Forest
- Conjunto de múltiplas árvores de decisão que trabalham em paralelo, reduzindo o risco de sobreajuste (overfitting) e melhorando a precisão das previsões. É robusto e oferece boa interpretabilidade por meio da importância das variáveis.

### 3. Elastic Net
- Modelo linear que combina as penalizações L1 (Lasso) e L2 (Ridge), controlando a complexidade do modelo e selecionando variáveis relevantes. É útil em situações onde há colinearidade entre os preditores.

### 4. Gradient Boosting Regressor
- Técnica baseada em aprendizado por reforço sequencial, onde novas árvores são adicionadas para corrigir os erros das anteriores. É um dos métodos mais poderosos para tarefas de regressão tabular.

### 5. Ridge Regression
- Regressão linear com regularização L2, que reduz a influência de variáveis altamente correlacionadas e melhora a estabilidade do modelo, evitando o sobreajuste.

---

## Justificativa Teórica

De acordo com o artigo [“Factors Affecting Students’ Performance: A Case of Students of Business Studies Faculty, King Abdulaziz University”](https://d1wqtxts1xzle7.cloudfront.net/56029351/student_performance-libre.pdf?1520838052=&response-content-disposition=inline%3B+filename%3DFACTORS_AFFECTING_STUDENTS_PERFORMANCE_A.pdf&Expires=1762262472&Signature=EO7IVnM7IJzBVzdc~Tbm9dVFIa7t8gXxGqD1VkN0T9Anc7c5HYW9D8clsvk~w9l81HII8RRv3nkI33kEBQinhUsiB770DB8D4GYy8Kyw2diNKbl1Yp9y5sfHnXgJPmDFb74OHOjbm0y95dEv4WSSIDNbATByKkkb4GGw7qu1kv1~yn7DYlPDXqJdnwDv-nawm68fuJNZjemduXG1nhZ1g1qXwWhmOjE3zv8zW8n5Qbpi~3zkSUwNr90OFDcSOXwKqCPYNDHoUYH7Sj4uWPHl1tWGCvBPkHEggSHDI1935aok4tg7XehcDcOh76P276qykZ-55TaMtpOHBSIqELt-JA__&Key-Pair-Id=APKAJLOHF5GGSLRBV4ZA), o desempenho acadêmico é um fenômeno **multifatorial**, influenciado tanto por aspectos **individuais** (como tempo de estudo, sono e motivação) quanto **externos** (como suporte familiar e ambiente escolar).

A aplicação de **modelos de aprendizado de máquina** neste contexto permite **quantificar o impacto de cada variável**, fornecendo previsões mais robustas e insights explicativos sobre a dinâmica do aprendizado — um avanço em relação às abordagens puramente estatísticas tradicionais.

---

## Referências

- **KAGGLE.** *Student Performance Factors Dataset.* Disponível em: [https://www.kaggle.com/datasets](https://www.kaggle.com/datasets).  
  Acesso em: 12 jun. 2025.

- **ALI, N. et al.** *Factors Affecting Students’ Performance: A Case of Students of Business Studies Faculty, King Abdulaziz University.*  
  *Research Journal of International Studies*, n. 12, p. 1–10, 2013.  
  Disponível em: [link do artigo].  
  Acesso em: 12 jun. 2025.

- **GERON, A.** *Hands-On Machine Learning with Scikit-Learn, Keras & TensorFlow.* 3ª ed. O’Reilly Media, 2022.

- **SCIKIT-LEARN Developers.** *Scikit-learn Documentation.*  
  Disponível em: [https://scikit-learn.org/stable/documentation.html](https://scikit-learn.org/stable/documentation.html).  
  Acesso em: 10 jun. 2025.

- Materiais de aula do professor Daniel R. Cassar

---

## Professor Orientador

| Professor | GitHub |
|------------|--------|
| **Prof. Dr. Daniel R. Cassar** | [@drcassar](https://github.com/drcassar) | |

---

## Contribuição da Equipe

| Integrante | GitHub |
|-------------|--------|
| **Gisela C. Kassick** | [@GiselaCK](https://github.com/GiselaCK) |
| **Giovani M. Nagano** | [@giovaninagano5](https://github.com/giovaninagano5) | 
| **Rebeka L. Batichotti** | — |

> Todos os membros participaram colaborativamente na elaboração dos códigos, apresentação e README do projeto.

