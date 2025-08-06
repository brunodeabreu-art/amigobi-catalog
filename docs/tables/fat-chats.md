# Tabela: fat_chats

## Descrição
Fato de conversas - registra todas as conversas e mensagens do sistema

## Informações Gerais
- **Tipo**: BASE TABLE
- **Total de Colunas**: 8
- **Colunas Sensíveis**: 1

## Estrutura das Colunas

| Nome da Coluna | Tipo | Nulo | Padrão | Descrição | Sensível |
|----------------|------|------|--------|-----------|----------|
| company_id | integer | Sim | - | Identificador único | Não |
| user_id | integer | Sim | - | Identificador único | Não |
| data_referencia | timestamp without time zone | Sim | - | Data dereferencia | Não |
| type | text | Sim | - | Campo de texto longo | Não |
| qtd_chat | bigint | Sim | - | Número inteiro longo | Não |
| qtd_request | bigint | Sim | - | Número inteiro longo | Não |
| qtd_files | bigint | Sim | - | Número inteiro longo | Não |
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
