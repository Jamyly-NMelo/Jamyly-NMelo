# Melhores Compras | Arquitetura Big Data e Bancos NoSQL

> **Tipo:** projeto acadêmico / proposta de arquitetura. Este documento descreve a solução apresentada no trabalho; não afirma que a arquitetura tenha sido implantada em produção.

## Visão geral

Estudo de arquitetura de dados para um cenário de e-commerce, considerando necessidades de catálogo, estoque, recomendação de produtos e análise de eventos relacionados à jornada de compra.

## Problema e contexto

O material fornecido descreve desafios associados a abandono de carrinho e à necessidade de organizar grandes volumes de dados. Qualquer percentual de abandono mencionado no trabalho deve ser acompanhado da fonte e do contexto originais antes de ser publicado como fato.

## Arquitetura proposta

### Seleção de bancos NoSQL por cenário

- **Banco orientado a grafos:** considerado para representar relações e conexões úteis à recomendação de produtos.
- **Banco colunar:** considerado para cenários de estoque e consultas analíticas.
- **Banco orientado a documentos:** considerado para catálogo com atributos flexíveis.

### Ingestão e processamento

A proposta descrita no material contempla:

- Apache NiFi para ingestão de arquivos de log.
- HDFS, HBase e Apache Pig na camada de processamento em lote.
- Apache Spark para processamento de eventos em tempo próximo ao real.
- Looker e Salesforce Marketing Cloud na camada de visualização e automação.

**Importante:** manter esses componentes como arquitetura proposta, a menos que os arquivos comprovem implementação e execução prática.

### Organização do Data Lake

Zonas citadas na proposta:

- `raw`
- `transient`
- `trusted`
- `curated`
- `sandbox`

O material também menciona classificação de dados em categorias como mestre, referência, transação e PII. A documentação final deve explicar as regras de acesso, retenção e proteção aplicáveis.

## Entregáveis

- [ ] Matriz comparativa dos bancos NoSQL
- [ ] Diagrama da arquitetura Lambda
- [ ] Diagrama das zonas do Data Lake
- [ ] Apresentação ou documento das fases do PBL

## Resultados e aprendizados

Descrever aqui as decisões arquiteturais justificadas no trabalho, as vantagens e limitações consideradas e os aprendizados obtidos. Evitar apresentar benefícios esperados como resultados medidos.

## Como reproduzir

Este é um registro de uma proposta acadêmica. Incluir instruções de execução somente se houver código, ambiente ou infraestrutura efetivamente disponibilizados.

## Fontes e créditos

Adicionar referências bibliográficas, documentação técnica e identificação do grupo conforme as regras da instituição. Não publicar matrículas ou dados pessoais dos integrantes.
