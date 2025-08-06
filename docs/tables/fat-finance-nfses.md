# Tabela: fat_finance_nfses

## Descrição
Fato financeiro de NFSes - registra notas fiscais de serviço emitidas

## Informações Gerais
- **Tipo**: BASE TABLE
- **Total de Colunas**: 10
- **Colunas Sensíveis**: 0

## Estrutura das Colunas

| Nome da Coluna | Tipo | Nulo | Padrão | Descrição | Sensível |
|----------------|------|------|--------|-----------|----------|
| id | integer | Sim | - | Identificador único | Não |
| servico_valores_valor_servicos | character varying(255) | Sim | - | Valor deservico_valores_servicos | Não |
| status | character varying(30) | Sim | - | Status atual | Não |
| created_at | timestamp without time zone | Sim | - | Data e hora de criação | Não |
| user_id | integer | Sim | - | Identificador único | Não |
| source | character varying(255) | Sim | - | Campo de texto variável | Não |
| new_attendance_id | integer | Sim | - | Identificador único | Não |
| company_id | integer | Sim | - | Identificador único | Não |
| dt_emissao | timestamp without time zone | Sim | - | Data deemissao | Não |
| dt_competencia | timestamp without time zone | Sim | - | Data decompetencia | Não |

## Relacionamentos
Esta tabela faz parte do sistema **data-warehouse** do AmigoBI.

## Última Atualização
Documentação gerada automaticamente em 06/08/2025.
