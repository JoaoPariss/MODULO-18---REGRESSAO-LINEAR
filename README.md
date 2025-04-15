# MODULO-18---REGRESSAO-LINEAR

# 📊 Previsão de Aluguel de Imóveis com Regressão Linear

Este projeto tem como objetivo aplicar regressão linear simples e múltipla para prever o preço de aluguel de imóveis com base em variáveis como metragem, número de quartos, vagas, banheiros, suítes e valor do condomínio.

Atividades realizadas: 
## 1. 📦 Entendimento e Pré-Processamento Inicial dos Dados
### A) Verificação dos Tipos de Dados.
### B) Verificação de Dados Faltantes

---

## 2. 🔍 Análise Exploratória e Pré-Processamento Intermediário
### A) Estatísticas Descritivas
- Utilização do `.describe()` para identificar outliers e entender a distribuição das variáveis.

### B) Análise Bivariada
Foram gerados 3 gráficos para analisar a relação entre variáveis independentes e o valor do aluguel:
1. Relação entre N_banheiros e Valor_Aluguel
2. Relação entre N_Suites e Valor_Aluguel
3. Relação entre N_Vagas e Valor_Aluguel
   
---

## 3. ✂️ Separação entre Treino e Teste + Regressão Linear Simples

### A) Separação da base
- Dados separados em `X_train`, `X_test`, `y_train`, `y_test` utilizando `train_test_split`.

### B) Regressão Linear Simples
- Treinamento do modelo com a variável `metragem` como única feature.
- Impressão dos valores de `intercept_` e `coef_`, com construção da equação da reta:
- ### C) Avaliação do Modelo
- Cálculo do **R²** para os dados de treino.
- O valor de R² foi interpretado com base na explicação da variância dos dados.

### D) Visualização
- Gráfico da reta de regressão linear sobre os pontos reais do conjunto de treino.
- Análise da dispersão dos pontos e aderência da reta ao padrão dos dados.

### E) Aplicação à base de teste
- Avaliação do modelo nos dados de teste.
- Comparação entre desempenho em treino e teste.

---

## 4. 🤖 Regressão Linear Múltipla

### A) Separação da base com todas as variáveis
- Foram utilizadas como variáveis independentes:
`Metragem`, `Valor_Condominio`, `N_Quartos`, `N_banheiros`, `N_Suites`, `N_Vagas`

### B) Treinamento do modelo com múltiplas variáveis
- Modelo treinado com `X_train` e `y_train`.

### C) Avaliação com R² nos dados de treino
- O modelo obteve um R² mais alto do que na regressão simples, indicando maior capacidade de explicação.

### D) Aplicação e avaliação no conjunto de teste
- R² calculado para os dados de teste.

### E) Comparação entre os modelos
