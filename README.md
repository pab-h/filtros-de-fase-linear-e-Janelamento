# Filtros de Fase Linear usando Janelamento

Este repositório contém a implementação completa do **Trabalho AP2** da disciplina **Processamento Digital de Sinais (SBL0085)**, ministrada pelo Prof. **C. Alexandre Rolim Fernandes**, no curso de **Engenharia da Computação** da **Universidade Federal do Ceará – Campus Sobral**.

O trabalho aborda a análise, projeto e comparação de filtros digitais **FIR** e **IIR**, com ênfase em **fase linear**, **atraso de grupo** e **métodos de janelamento**.

## 📌 Objetivos do Trabalho

- Analisar sinais no domínio do tempo e da frequência
- Projetar filtros **FIR passa-baixa** por janelamento (Retangular e Kaiser)
- Projetar filtros **IIR passa-baixa Butterworth**
- Avaliar:
  - Resposta em magnitude
  - Resposta em fase
  - Atraso de grupo
- Comparar os efeitos de **fase linear** e **fase não linear**
- Verificar o comportamento do sinal filtrado
- Analisar o diagrama de **polos e zeros** de filtros FIR


## 📂 Estrutura do Código

Todo o trabalho foi implementado em **um único arquivo**, conforme solicitado no enunciado, organizado em seções:

```

├── Parte 1 — Filtro FIR com Janela Retangular
│   ├── Geração do sinal x[n]
│   ├── FFT do sinal
│   ├── Projeto do filtro FIR ideal truncado
│   ├── Resposta em frequência, fase e atraso de grupo
│   └── Filtragem do sinal
│
├── Parte 2 — Filtro IIR Butterworth
│   ├── Projeto do filtro Butterworth (ordem 8)
│   ├── Resposta em frequência
│   ├── Resposta em fase
│   ├── Atraso de grupo
│   └── Filtragem do sinal e análise do atraso
│
├── Parte 3 — Filtro FIR por Janelamento
│   ├── Projeto com Janela clássica (Hamming)
│   ├── Projeto com Janela de Kaiser
│   ├── Comparação das ordens
│   ├── Resposta em frequência, fase e atraso de grupo
│   ├── Filtragem do sinal
│   └── Diagrama de polos e zeros

```


## 📊 Principais Resultados

- O filtro **FIR com janela retangular** apresenta:
  - Fase linear
  - Atraso de grupo constante
  - Lóbulos laterais elevados na banda de rejeição

- O filtro **IIR Butterworth** apresenta:
  - Resposta em magnitude maximamente plana
  - Fase não linear
  - Atraso de grupo variável

- O filtro **FIR com janela de Kaiser** apresenta:
  - Maior flexibilidade no projeto (parâmetro β)
  - Melhor compromisso entre largura da transição e atenuação
  - Fase aproximadamente linear na banda de passagem

- O diagrama de **polos e zeros** do filtro FIR mostra:
  - Polos apenas na origem (característica FIR)
  - Zeros próximos à circunferência unitária nas bandas de rejeição
  - Estrutura compatível com filtros FIR de fase linear

