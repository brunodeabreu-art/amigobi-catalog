# Tabela: fat_attendance_records

## Descrição
Fato de registros de atendimento - armazena histórico de atendimentos realizados

## Informações Gerais
- **Tipo**: BASE TABLE
- **Total de Colunas**: 8
- **Colunas Sensíveis**: 1

## Estrutura das Colunas

| Nome da Coluna | Tipo | Nulo | Padrão | Descrição | Sensível |
|----------------|------|------|--------|-----------|----------|
| user_id | integer | Não | - | Identificador único | Não |
| company_id | integer | Não | - | Identificador único | Não |
| type | character varying(255) | Não | - | Campo de texto variável | Não |
| subtype | text | Não | - | Campo de texto longo | Não |
| has_digital_signature | boolean | Não | - | Valor verdadeiro/falso | Não |
| data_referencia | timestamp without time zone | Não | - | Data dereferencia | Não |
| qtd | bigint | Sim | - | Número inteiro longo | Não |
| dat_carga | timestamp without time zone | Sim | CURRENT_TIMESTAMP | Registro Geral - DADO SENSÍVEL | 🔒 Sim |

## ⚠️ Colunas Sensíveis (PII)

Esta tabela contém **1 coluna(s) sensível(is)** que requerem cuidados especiais:

- **dat_carga**: Registro Geral - DADO SENSÍVEL

### Políticas de Acesso
- Acesso restrito apenas a usuários autorizados
- Logs de auditoria obrigatórios
- Mascaramento de dados em ambientes de desenvolvimento
- Conformidade com LGPD

## Relacionamentos
Esta tabela faz parte do sistema **data-warehouse** do AmigoBI.

## Última Atualização
Documentação gerada automaticamente em 06/08/2025.
