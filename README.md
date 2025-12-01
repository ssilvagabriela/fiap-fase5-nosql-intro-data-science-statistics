# Fase 5 – NoSQL & Intro Data Science Statistics (FIAP)

## Sobre o Projeto

Esta fase conectou dois pilares fundamentais do curso de Data Science:

* **NoSQL e Arquitetura de Dados Não Relacionais**,
* **Estatística aplicada em Python**, com foco em análise exploratória e interpretação quantitativa.

A atividade da fase foi dividida em **duas entregas principais**:

1. **Prova de Conceito (PoC) de bases NoSQL**, avaliando cenários reais da Melhores Compras LTDA.
2. **Análise Estatística de vendas com Python**, incluindo outliers, médias, dispersão e correlações.

---

# Estrutura do Repositório

```
/python
   Grupo21_PBL_TSCO_1o_Ano_Fase5.ipynb   → Notebook com análises estatísticas e visualizações

/docs
   Grupo21_PBL_TSCO_1o_Ano_Fase5.pdf     → Relatório completo: NoSQL + Estatística
```

---

# Prova de Conceito – Banco de Dados NoSQL

Com base nos cenários apresentados, o grupo avaliou problemas reais de desempenho e propôs soluções NoSQL adequadas:

### **Cenário 1 – Recomendações de produto**

→ **Banco escolhido:** Grafo (Neo4j)
→ Justificativa: relações complexas entre clientes e produtos, recomendação baseada em compras correlatas, alto volume de dados.
→ Referência: Facebook utiliza grafos para modelar conexões.

---

### **Cenário 2 – Estoque para entrega 24h**

→ **Banco escolhido:** Colunar (Cassandra)
→ Justificativa: leituras rápidas por coluna, baixa latência, alta escalabilidade em inventário.
→ Referência: Walmart utiliza Cassandra para estoque global em tempo real.

---

### **Cenário 3 – Tela de detalhes do produto**

→ **Banco escolhido:** Documento (MongoDB)
→ Justificativa: flexibilidade para armazenar JSONs com reviews, versões, imagens e atributos dinâmicos.
→ Referência: Sephora usa MongoDB para catálogo de produtos variados.

---

# Análise Estatística – Python

A segunda parte do trabalho envolveu analisar dados de vendas usando Python:

Notebook: **Grupo21_PBL_TSCO_1o_Ano_Fase5.ipynb**

As etapas incluíram:

---

### **Outliers (Quantidade de produtos)**

O boxplot da página 6 mostra forte presença de outliers, chegando a quantidades acima de 100 unidades por compra.
Após winsorização:

* desvio padrão caiu de **≈ 12** para **≈ 0,82**
* distribuição ficou mais estável

Interpretação: outliers representam compras B2B.

---

### **Diferenças de preço entre regiões**

Conclusão:
Não houve diferença estatística significativa entre regiões ou formas de pagamento.
Variações próximas de **±1%**.

---

### **Correlações**

A matriz de correlação (página 9) indica:

* **Quantidade × Lucro_liquido = 0,56** (forte positiva)
* **Valor_comissão × Lucro_liquido = 0,89** (muito forte)

---

# Principais Aprendizados da Fase

> Identificar quando modelos relacionais deixam de ser eficientes
> Selecionar bancos NoSQL adequados para cada tipo de demanda
> Conduzir provas de conceito orientadas por cenários reais
> Detectar e tratar outliers com técnicas estatísticas
> Comparar médias e interpretar diferenças de preço
> Criar matrizes de correlação e visualizar padrões
> Utilizar Pandas, NumPy e Matplotlib para análises profissionais

---

# Integrantes do Grupo

* Carlos Vinícius Rodrigues Silva
* Gabriela Sena da Silva
* Gustavo Almeira Scardini
* Tatiana Espinola
* Vitor Fernandes Antunes

---

# 📩 Contato

**Gabriela Sena da Silva**

🔗 LinkedIn: [https://www.linkedin.com/in/gabrielasena](https://www.linkedin.com/in/gabrielasena)

📧 [gabisena@outlook.com](mailto:gabisena@outlook.com)


Se quiser conversar sobre NoSQL, Estatística, Python ou Data Architecture, será um prazer ajudar!
