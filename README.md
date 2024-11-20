
# CreditRiskPrediction

## Introdução
Este repositório contém as análises e implementações desenvolvidas durante projeto do Módulo 07 do curso profissionalizante de Cientista de Dados da EBAC. O objetivo principal foi preparar uma base de dados, realizar manipulações para adequação a ferramentas como Scikit-Learn e implementar modelos de aprendizado de máquina, avaliando a performance em diferentes cenários.


## 📁 Estrutura dos Projetos

### **Módulo 07 - Tarefa 01: Preparação e Análise de Dados**
Neste projeto, trabalhamos com a base de dados `demo01.csv`, realizando uma série de etapas fundamentais para a modelagem:

- **Carregamento e Exploração Inicial:**
  - Avaliação de variáveis e tipos de dados.
  - Identificação de valores ausentes.
  - Análise da distribuição da variável resposta (`mau`).

- **Criação de Metadados:**
  - Construção de um DataFrame descritivo contendo:
    - Nome das variáveis.
    - Tipos de dados.
    - Quantidade de categorias para variáveis qualitativas.

- **Transformação de Dados:**
  - Geração de variáveis dummy para variáveis categóricas.
  - Ajuste dos dados para entrada no Scikit-Learn.

- **Insights sobre Variáveis Importantes:**
  - Análise de cruzamento entre `possui_email` e `posse_de_veiculo` com a variável resposta, identificando padrões que ajudam na modelagem.

**Resultado:** A base foi ajustada e salva como `Projeto_mod07.csv` para uso em tarefas futuras.

---

### **Módulo 07 - Tarefa 02: Modelagem com Árvores de Decisão**
Construção e avaliação de modelos preditivos para classificar contratos como aprovados ou reprovados:

- **Preparação de Dados:**
  - Divisão da base em treinamento (70%) e validação (30%).
  - Exclusão de variáveis em formato string.

- **Modelagem Inicial:**
  - Treinamento de uma árvore de decisão simples.
  - Avaliação da acurácia e visualização da matriz de confusão.

- **Ajuste de Hiperparâmetros:**
  - Construção de uma nova árvore com:
    - Mínimo de 5 observações por folha.
    - Profundidade máxima de 10.
  - Comparação dos resultados com a árvore inicial.

- **Resultados:**
  - **Acurácia na Base de Treinamento:** 99.12%.
  - **Acurácia na Base de Teste:** 97.52%.
  - **Proporção de Maus Classificados:** 0.64%.

- **Conclusões:**
  - Testamos a acurácia do modelo em diferentes cenários, incluindo a hipótese de classificar todos os contratos como `bons`, que gerou uma acurácia de 97.84%. Isso destaca a importância de considerar o impacto real dos erros no negócio.

---

## 🛠️ Tecnologias Utilizadas

- **Linguagem de Programação:** Python
- **Bibliotecas:** 
  - Pandas
  - NumPy
  - Scikit-learn
  - Matplotlib
- **Ferramentas de Visualização:** Visualização de árvores e matrizes de confusão.

---

## 📊 Principais Lições

1. **Preparação de Dados é Essencial:**
   A análise inicial, criação de variáveis dummy e tratamento de missings são etapas críticas para garantir a eficácia do modelo.

2. **Acurácia Não é Tudo:**
   Avaliar a proporção de erros e o impacto no negócio é tão importante quanto o índice de acurácia.

3. **Modelos Ajustados Performam Melhor:**
   Pequenos ajustes nos hiperparâmetros de uma árvore de decisão podem gerar ganhos significativos em performance.

---

## Sinta-se à vontade para explorar, contribuir ou utilizar os códigos e ideias presentes neste repositório! 🚀

