# Otimização de Estoque de Varejo com Python

**Tipo:** Otimização / Pesquisa Operacional
**Dataset:** [Online Retail II - UCI](https://archive.ics.uci.edu/ml/datasets/Online+Retail+II)

## O Desafio
Equilibrar o *trade-off* entre **Nível de Serviço** (disponibilidade para o cliente) e **Custo de Estoque**. O projeto foca em um produto de alta volatilidade (*Lumpy Demand*) onde médias simples falham.

## A Solução Técnica
Utilizei Python para implementar algoritmos de Gestão de Estoques "do zero" (sem depender de caixas pretas):
* **Limpeza de Dados:** Tratamento de devoluções e filtragem geográfica (Reino Unido).
* **Análise Estatística:** Identificação de sazonalidade e cálculo de CV (Coeficiente de Variação).
* **Modelo Matemático:** Implementação das fórmulas de **EOQ (Lote Econômico)** e **Safety Stock (Estoque de Segurança)** probabilístico.

## Resultados
Para garantir 95% de atendimento aos pedidos:
* **Gatilho de Compra:** 1690 unidades.
* **Lote de Compra:** 532 unidades.
* **Impacto:** Identifiquei que o Estoque de Segurança custa **~£12.700/ano** para este único item. O projeto fornece a base quantitativa para decidir se vale a pena manter esse nível de serviço ou renegociar o Lead Time.

---
**Autor:** Davi Duarte Cucco
*Conectando Data Science e Engenharia de Produção* | [LinkedIn](https://www.linkedin.com/in/davi-duarte-cucco-8b272a238)
