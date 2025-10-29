# Data Processing Case

Este projeto analisa dados do Airbnb do Rio de Janeiro, extraindo insights sobre amenidades e seus impactos nos preços.

## Configuração do Ambiente

### 1. Chave da API OpenAI

Para executar o processamento de dados que utiliza modelos de linguagem, você precisa configurar sua chave da API OpenAI:

1. Crie uma conta em [OpenAI](https://platform.openai.com/)
2. Gere uma chave de API
3. Configure a variável de ambiente:
   ```bash
   export OPENAI_API_KEY="sua_chave_aqui"
   ```

### 2. Download dos Dados

Os dados brutos não estão incluídos no repositório. Você precisa baixá-los manualmente:

1. Acesse [Inside Airbnb](https://insideairbnb.com/get-the-data/)
2. Procure pela cidade **Rio de Janeiro, Rio de Janeiro, Brazil**
3. Baixe os seguintes arquivos da data mais recente disponível:
   - `reviews.csv.gz` 
   - `listings.csv.gz`
4. Descompacte os arquivos e coloque-os na pasta `data/raw/` com os nomes:
   - `data/raw/reviews.csv`
   - `data/raw/listings.csv`

### 3. Estrutura de Pastas

Após o download, sua estrutura deve ficar assim:
```
data/
├── raw/
│   ├── reviews.csv
│   └── listings.csv
└── processed/
    └── (arquivos processados serão gerados aqui)
```

## Executando o Projeto

1. Certifique-se de ter as dependências instaladas
2. Configure a chave da API OpenAI
3. Baixe os dados conforme instruções acima
4. Execute os scripts de processamento

## Dados Processados

O projeto gera os seguintes arquivos na pasta `data/processed/`:
- Análises de amenidades extraídas dos comentários
- Impacto das amenidades nos preços
- Dados limpos e estruturados para análise