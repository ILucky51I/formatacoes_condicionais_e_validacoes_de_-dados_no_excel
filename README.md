# Análise de Pessoas por Faixa de Impostos

Projeto de análise de dados desenvolvido a partir de um dataset contendo informações sobre contribuintes, renda declarada, impostos, situação fiscal, fonte de renda e distribuição por estado.

O objetivo do projeto é explorar os dados e identificar a distribuição de pessoas entre diferentes **faixas de imposto**, analisando também possíveis relações com **fonte de renda** e **estado**.

---

## Sobre o Projeto

Este projeto apresenta uma análise exploratória de um conjunto de **300 registros de contribuintes**.

A base contém informações financeiras e cadastrais utilizadas para gerar uma visão consolidada da distribuição dos contribuintes por faixa de imposto.

O arquivo também possui uma aba de **Report**, contendo tabelas consolidadas para análise por:

- Faixa de imposto;
- Fonte de renda;
- Estado;
- Quantidade de contribuintes.

---

## Objetivos

- Analisar a quantidade de pessoas em cada faixa de imposto;
- Identificar a distribuição dos contribuintes por fonte de renda;
- Analisar a distribuição das faixas de imposto entre os estados;
- Organizar os dados para facilitar a interpretação;
- Desenvolver uma análise exploratória utilizando dados tabulares;
- Criar uma base que possa posteriormente ser utilizada para dashboards e outras análises.

---

## Dataset

O dataset possui **300 registros** e **19 colunas**.

### Principais campos

| Campo | Descrição |
|---|---|
| `Contribuinte ID` | Identificador do contribuinte |
| `Nome` | Nome do contribuinte |
| `CPF` | Documento cadastral |
| `Ano Referência` | Ano de referência da declaração |
| `Renda Declarada(R$)` | Valor da renda declarada |
| `Imposto Devido(R$)` | Valor do imposto devido |
| `Imposto Pago(R$)` | Valor efetivamente pago |
| `Valor Não Declarado(R$)` | Valor identificado como não declarado |
| `Déficit Declaração(%)` | Percentual de déficit na declaração |
| `Situação` | Situação da declaração |
| `Data Envio` | Data de envio da declaração |
| `Estado` | Estado do contribuinte |
| `Fonte de Renda` | Principal fonte de renda |
| `Número de Bens Declarados` | Quantidade de bens declarados |
| `Total de Deduções(R$)` | Total de deduções |
| `Imposto Restituição(R$)` | Valor de restituição |
| `Faixa Imposto` | Faixa de imposto do contribuinte |
| `Recebeu Multas?` | Indica se recebeu multa |
| `Valor Multas(R$)` | Valor das multas |

---

## Faixas de Imposto

A análise apresenta cinco categorias de faixa de imposto:

| Faixa | Quantidade |
|---|---:|
| 7,5% | 58 |
| 15% | 62 |
| 22,5% | 61 |
| 27,5% | 58 |
| Isento | 61 |
| **Total** | **300** |

A distribuição demonstra que os registros estão relativamente distribuídos entre as diferentes categorias analisadas.

A faixa de **15% possui 62 registros**, enquanto as faixas de **22,5% e Isento possuem 61 registros cada**.

---

## Distribuição por Fonte de Renda

A base contempla diferentes fontes de renda:

- Aposentado;
- Autônomo;
- Empregado CLT;
- Empresário;
- Investidor.

A aba de relatório permite cruzar a **fonte de renda** com a **faixa de imposto**, possibilitando análises como:

> Quantos investidores estão na faixa de 27,5%?

> Quantos empregados CLT são isentos?

> Qual é a distribuição dos autônomos entre as faixas de imposto?

---

## Distribuição por Estado

Os registros também podem ser analisados por estado, permitindo comparar a distribuição das faixas de imposto entre diferentes unidades federativas.

Entre os estados presentes na base estão:

- Amazonas (AM)
- Bahia (BA)
- Ceará (CE)
- Distrito Federal (DF)
- Espírito Santo (ES)
- Goiás (GO)
- Minas Gerais (MG)
- Mato Grosso (MT)
- Paraíba (PB)
- Pernambuco (PE)
- Paraná (PR)
- Rio de Janeiro (RJ)
- Rio Grande do Sul (RS)
- Santa Catarina (SC)
- São Paulo (SP)

Essa dimensão permite realizar análises geográficas e identificar como os contribuintes estão distribuídos entre as diferentes faixas.

---

## Estrutura do Arquivo

```text
Quantidade de Pessoas Por Faixa de Impostos.xlsx
│
├── dataset_impostos_case_situation
│   └── Base principal com 300 registros
│
└── Report
    ├── Quantidade por Faixa de Imposto
    ├── Quantidade por Fonte de Renda
    └── Quantidade por Estado
