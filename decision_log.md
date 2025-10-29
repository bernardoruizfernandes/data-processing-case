# Decision Log - Análise Airbnb

## Decisões Técnicas

### Stack de Dados
- **Pandas + NumPy**: Volume de 1.384 listings cabe em memória, pandas ideal para análise exploratória
- **Claude API**: Extração de amenities dos comentários usando IA
- **Batch Processing**: 10 comentários por requisição, respeitando limite de 50 req/min

### Metodologia
- **Filtragem geográfica**: Foco em Leblon apenas (demonstração)
- **Sentiment Analysis**: Classificação automática positivo/negativo/neutro
