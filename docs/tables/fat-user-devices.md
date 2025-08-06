# Tabela: fat_user_devices

## Descrição
Fato de dispositivos de usuário - registra dispositivos utilizados pelos usuários

## Informações Gerais
- **Tipo**: BASE TABLE
- **Total de Colunas**: 13
- **Colunas Sensíveis**: 1

## Estrutura das Colunas

| Nome da Coluna | Tipo | Nulo | Padrão | Descrição | Sensível |
|----------------|------|------|--------|-----------|----------|
| id | integer | Sim | - | Identificador único | Não |
| user_id | integer | Sim | - | Identificador único | Não |
| id_aparelho | character varying(255) | Sim | - | Identificador único | Não |
| marca | character varying(255) | Sim | - | Campo de texto variável | Não |
| aparelho | character varying(255) | Sim | - | Campo de texto variável | Não |
| modelo | character varying(255) | Sim | - | Campo de texto variável | Não |
| fabrica | character varying(255) | Sim | - | Campo de texto variável | Não |
| versao | character varying(255) | Sim | - | Campo de texto variável | Não |
| tipo | character varying(255) | Sim | - | Campo de texto variável | Não |
| sistema | character varying(255) | Sim | - | Campo de texto variável | Não |
| versao_sistema | character varying(255) | Sim | - | Campo de texto variável | Não |
| status | character varying(255) | Sim | - | Status atual | Não |
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
