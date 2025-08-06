# Tabela: fat_posts

## Descrição
Fato de posts - armazena publicações e conteúdos criados pelos usuários

## Informações Gerais
- **Tipo**: BASE TABLE
- **Total de Colunas**: 20
- **Colunas Sensíveis**: 0

## Estrutura das Colunas

| Nome da Coluna | Tipo | Nulo | Padrão | Descrição | Sensível |
|----------------|------|------|--------|-----------|----------|
| id | integer | Sim | - | Identificador único | Não |
| text | text | Sim | - | Campo de texto longo | Não |
| total_likes | integer | Sim | - | Valor total | Não |
| total_comments | integer | Sim | - | Valor total | Não |
| total_shares | integer | Sim | - | Valor total | Não |
| profile_id | integer | Sim | - | Identificador único | Não |
| creator_id | integer | Sim | - | Identificador único | Não |
| link_id | integer | Sim | - | Identificador único | Não |
| is_sponsored | boolean | Sim | - | Indicador booleanosponsored | Não |
| is_deleted | boolean | Sim | - | Indicador booleanodeleted | Não |
| created_at | timestamp without time zone | Sim | - | Data e hora de criação | Não |
| updated_at | timestamp without time zone | Sim | - | Data e hora da última atualização | Não |
| parent_post_id | integer | Sim | - | Identificador único | Não |
| title | character varying(255) | Sim | - | Campo de texto variável | Não |
| external_post_key | character varying(255) | Sim | - | Campo de texto variável | Não |
| summary | text | Sim | - | Campo de texto longo | Não |
| status | character varying(20) | Sim | - | Status atual | Não |
| destroyer_id | integer | Sim | - | Identificador único | Não |
| available_at | timestamp without time zone | Sim | - | Campo do tipo timestamp without time zone | Não |
| cover_image_url | character varying(255) | Sim | - | Campo de texto variável | Não |

## Relacionamentos
Esta tabela faz parte do sistema **data-warehouse** do AmigoBI.

## Última Atualização
Documentação gerada automaticamente em 06/08/2025.
