# Tabela: dim_user

## Descrição
Dimensão de usuários - contém dados mestres dos usuários do sistema

## Informações Gerais
- **Tipo**: BASE TABLE
- **Total de Colunas**: 23
- **Colunas Sensíveis**: 2

## Estrutura das Colunas

| Nome da Coluna | Tipo | Nulo | Padrão | Descrição | Sensível |
|----------------|------|------|--------|-----------|----------|
| user_id | bigint | Não | nextval('dim_user_user_id_seq'::regclass) | Identificador único | Não |
| user_name | text | Sim | - | Campo de texto longo | Não |
| specialty_name | text | Sim | - | Campo de texto longo | Não |
| gender | character varying(25) | Sim | - | Campo de texto variável | Não |
| address_city | character varying(255) | Sim | - | Campo de texto variável | Não |
| address_state | character varying(255) | Sim | - | Campo de texto variável | Não |
| created_at | timestamp without time zone | Sim | - | Data e hora de criação | Não |
| updated_at | timestamp without time zone | Sim | - | Data e hora da última atualização | Não |
| dat_carga | timestamp without time zone | Sim | - | Registro Geral - DADO SENSÍVEL | 🔒 Sim |
| is_deleted | boolean | Sim | - | Indicador booleanodeleted | Não |
| born | date | Sim | - | Data | Não |
| ind_amigo_one | boolean | Sim | - | Valor verdadeiro/falso | Não |
| is_active | text | Sim | - | Indicador booleanoactive | Não |
| birdid_token | character varying(255) | Sim | - | Identificador único | Não |
| email | text | Sim | - | Endereço de email - DADO SENSÍVEL | 🔒 Sim |
| dt_last_login | timestamp without time zone | Sim | - | Data delast_login | Não |
| indication_code | character varying(6) | Sim | - | Campo de texto variável | Não |
| indicator_profile_id | integer | Sim | - | Identificador único | Não |
| indicator_name | text | Sim | - | Campo de texto longo | Não |
| ind_premium | boolean | Sim | - | Valor verdadeiro/falso | Não |
| profile_id | integer | Sim | - | Identificador único | Não |
| total_patients_created | bigint | Sim | - | Valor total | Não |
| is_certificado_ativo | boolean | Sim | - | Indicador se está ativo | Não |

## ⚠️ Colunas Sensíveis (PII)

Esta tabela contém **2 coluna(s) sensível(is)** que requerem cuidados especiais:

- **dat_carga**: Registro Geral - DADO SENSÍVEL
- **email**: Endereço de email - DADO SENSÍVEL

### Políticas de Acesso
- Acesso restrito apenas a usuários autorizados
- Logs de auditoria obrigatórios
- Mascaramento de dados em ambientes de desenvolvimento
- Conformidade com LGPD

## Relacionamentos
Esta tabela faz parte do sistema **data-warehouse** do AmigoBI.

## Última Atualização
Documentação gerada automaticamente em 06/08/2025.
