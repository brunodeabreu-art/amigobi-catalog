# Tabela: fat_conexoes

## Descrição
Fato de conexões - monitora conexões e sessões de usuários

## Informações Gerais
- **Tipo**: BASE TABLE
- **Total de Colunas**: 6
- **Colunas Sensíveis**: 1

## Estrutura das Colunas

| Nome da Coluna | Tipo | Nulo | Padrão | Descrição | Sensível |
|----------------|------|------|--------|-----------|----------|
| data_referencia | timestamp without time zone | Sim | - | Data dereferencia | Não |
| status | character varying(255) | Sim | - | Status atual | Não |
| name | text | Sim | - | Campo de texto longo | Não |
| quantidade | double precision | Sim | - | Identificador único | Não |
| source_profile_id | integer | Sim | - | Identificador único | Não |
| target_profile_id | integer | Sim | - | Identificador único | 🔒 Sim |

## ⚠️ Colunas Sensíveis (PII)

Esta tabela contém **1 coluna(s) sensível(is)** que requerem cuidados especiais:

- **target_profile_id**: Identificador único

### Políticas de Acesso
- Acesso restrito apenas a usuários autorizados
- Logs de auditoria obrigatórios
- Mascaramento de dados em ambientes de desenvolvimento
- Conformidade com LGPD

## Relacionamentos
Esta tabela faz parte do sistema **data-warehouse** do AmigoBI.

## Última Atualização
Documentação gerada automaticamente em 06/08/2025.
