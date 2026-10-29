# Trabalho de Estatística — Parte 1

Trabalho extraclasse da disciplina **Estatística Básica para Computação (T2)** — UFPel / CDTec.

**Grupo 12:** Felipe Mareque e Miguel Müller da Rosa
**Entrega:** 18/11/2026

## Sobre

Análise de uma pesquisa sobre o impacto de diferentes arquiteturas de computadores no processamento de dados (78 execuções de teste).

- **Variáveis independentes (hardware):** tipo de tarefa (A), núcleos de CPU (B), memória RAM (C), tipo de armazenamento (D), co-processamento (E)
- **Variáveis dependentes (desempenho):** taxa de transferência em GB/s (X), consumo de processamento em % (Y), eficiência de memória em % (Z), tempo total de processamento em s (W)

O enunciado completo e os dados estão em [`Grupo_12_-_T1_-_Felipe_Mareque_e_Miguel_Muller_da_Rosa.pdf`](Grupo_12_-_T1_-_Felipe_Mareque_e_Miguel_Muller_da_Rosa.pdf).

## Questões

1. Unidade de observação e classificação das variáveis
2. Medidas descritivas das variáveis numéricas (média, variância, desvio padrão, CV, assimetria, curtose)
3. Tabela de médias de dupla entrada (ML Training: núcleos × armazenamento, para o consumo de processamento)
4. Resumo de cinco números, cercas, valores atípicos e box plot do tempo de processamento por capacidade de RAM
5. Tabela de frequências e histograma da eficiência de memória (SQL Query)

## Tecnologias

O trabalho será feito em **Python** (pandas, numpy, scipy, matplotlib).

## Estrutura

```
├── data/
│   └── dados.csv                    # 78 execuções transcritas do enunciado
├── src/
│   ├── carregar_dados.py            # leitura do CSV
│   ├── q1_classificacao.py
│   ├── q2_medidas_descritivas.py
│   ├── q3_tabela_dupla_entrada.py
│   ├── q4_boxplot.py
│   └── q5_histograma.py
├── outputs/
│   ├── figuras/                     # gráficos gerados (box plot, histograma)
│   └── tabelas/                     # tabelas geradas
├── main.py                          # executa todas as questões
└── requirements.txt
```

## Como executar

```bash
python -m venv .venv
.venv\Scripts\activate        # Windows
pip install -r requirements.txt
python main.py
```