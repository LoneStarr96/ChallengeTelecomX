# Challenge Telecom X

Challenge Alura-ONE Telecom X

# Análise de Churn - Telecom X

Este é um projeto de análise exploratória de dados para identificar os principais fatores de churn (cancelamento de clientes) na base Telecom X.

#### 1. Introdução
- Objetivo: entender os principais drivers de churn e gerar ações práticas para reduzir a evasão.
- Problema: churn alto gera perda de receita recorrente e aumenta o custo de aquisição de novos clientes.
- Pergunta central: **Por que os clientes estão cancelando e o que podemos fazer para retê-los?**

#### 2. Carregamento e ETL
- Fonte: arquivo JSON público (GitHub)
- Principais ações realizadas:
  - Leitura e normalização do JSON
  - Remoção de linhas com Churn vazio/inválido
  - Conversão de Churn ("Yes"/"No" → 1/0)
  - Conversão de valores monetários para numérico
  - Criação de faixas de tenure (customer_tenure agrupado)

#### 3. Análise Exploratória (EDA)
- Principais visualizações criadas:
  - Proporção geral de churn (pizza + barras)
  - Churn por tipo de contrato (barras)
  - Distribuição de cobrança mensal por churn (boxplot + médias)
  - Churn por tempo de permanência (faixas de tenure)
  - Heatmap de correlações (variáveis mais relevantes)

Principais achados:
- Taxa de churn ≈ 26,5%
- Maior risco: contratos **month-to-month** (~42–43%)
- Clientes que cancelam pagam em média **R$ 13–14 a mais por mês**
- Churn muito alto nos primeiros 6–12 meses

#### 4. Relatório Final
**Conclusões e insights principais**
- Contratos mensais são o maior driver de churn
- Preço percebido elevado aumenta significativamente o risco
- Primeiros meses são críticos (onboarding fraco → alta evasão)
- Serviços de proteção/suporte técnico reduzem churn
- Taxa geral de 26,5% é alta e exige ação urgente

**Recomendações práticas**
- Migrar clientes month-to-month para planos anuais com desconto
- Criar bundles atrativos de proteção + suporte técnico
- Reforçar ações de onboarding nos primeiros 90 dias
- Implementar modelo preditivo de churn (priorizar: tipo de contrato, valor mensal, tenure, serviços adicionais)
- Testar descontos direcionados para clientes acima de R$ 70–75/mês


Pronto para usar.  
Salve como `README.md` na raiz do repositório.
