# Tabela: dim_company

## Descrição
Dimensão de empresas - contém dados mestres das empresas cadastradas no sistema

## Informações Gerais
- **Tipo**: BASE TABLE
- **Total de Colunas**: 31
- **Colunas Sensíveis**: 4

## Estrutura das Colunas

| Nome da Coluna | Tipo | Nulo | Padrão | Descrição | Sensível |
|----------------|------|------|--------|-----------|----------|
| company_id | bigint | Não | nextval('dim_company_company_id_seq'::regclass) | Identificador único | Não |
| name | text | Sim | - | Campo de texto longo | Não |
| cnpj | character varying(255) | Sim | - | CNPJ da empresa - DADO SENSÍVEL | 🔒 Sim |
| contact_email | character varying(255) | Sim | - | Endereço de email - DADO SENSÍVEL | 🔒 Sim |
| contact_phone | character varying(25) | Sim | - | Campo de texto variável | Não |
| address_cep | character varying(25) | Sim | - | Campo de texto variável | Não |
| address_address | character varying(255) | Sim | - | Campo de texto variável | Não |
| address_number | character varying(255) | Sim | - | Campo de texto variável | Não |
| address_complement | character varying(255) | Sim | - | Campo de texto variável | Não |
| address_district | character varying(255) | Sim | - | Campo de texto variável | Não |
| address_city | character varying(255) | Sim | - | Campo de texto variável | Não |
| address_state | character varying(255) | Sim | - | Campo de texto variável | Não |
| active | boolean | Sim | - | Valor verdadeiro/falso | Não |
| fiscal_tax_regime | character varying(255) | Sim | - | Campo de texto variável | Não |
| fiscal_cpf_responsible | character varying(25) | Sim | - | CPF do usuário - DADO SENSÍVEL | 🔒 Sim |
| fiscal_razao_social | text | Sim | - | Campo de texto longo | Não |
| created_at | timestamp without time zone | Sim | - | Data e hora de criação | Não |
| updated_at | timestamp without time zone | Sim | - | Data e hora da última atualização | Não |
| code | character varying(25) | Sim | - | Campo de texto variável | Não |
| customer_responsible | character varying(255) | Sim | - | Campo de texto variável | Não |
| contract_start_date | timestamp without time zone | Sim | - | Campo do tipo timestamp without time zone | Não |
| type | character varying(2) | Sim | - | Campo de texto variável | Não |
| industry_type | character varying(255) | Sim | - | Campo de texto variável | Não |
| allow_send_new_patient_sms | boolean | Sim | - | Valor verdadeiro/falso | Não |
| allow_send_confirmation_sms | boolean | Sim | - | Valor verdadeiro/falso | Não |
| allow_send_medical_record_sms | boolean | Sim | - | Valor verdadeiro/falso | Não |
| allow_send_telemedicine_sms | boolean | Sim | - | Valor verdadeiro/falso | Não |
| is_personal | boolean | Sim | - | Indicador booleanopersonal | Não |
| dat_carga | timestamp without time zone | Sim | - | Registro Geral - DADO SENSÍVEL | 🔒 Sim |
| is_deleted | boolean | Sim | - | Indicador booleanodeleted | Não |
| config_modules | text | Sim | - | Campo de texto longo | Não |

## ⚠️ Colunas Sensíveis (PII)

Esta tabela contém **4 coluna(s) sensível(is)** que requerem cuidados especiais:

- **cnpj**: CNPJ da empresa - DADO SENSÍVEL
- **contact_email**: Endereço de email - DADO SENSÍVEL
- **fiscal_cpf_responsible**: CPF do usuário - DADO SENSÍVEL
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
