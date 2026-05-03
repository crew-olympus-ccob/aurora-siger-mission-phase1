# Missão Aurora Siger: Fase 1

## Introdução
Vivemos a "Nova Corrida Espacial", onde a exploração de Marte exige sistemas autônomos e resilientes. A **Missão Aurora Siger** simula o ecossistema de uma nave interplanetária, onde a computação embarcada atua como o sistema nervoso central. Este projeto automatiza o **Relatório Operacional de Pré-Decolagem** da nave Aurora, validando variáveis críticas de telemetria, realizando análises energéticas e lidando com dilemas de missão em tempo real.

## Objetivos do Projeto
* **Análise de Telemetria:** Processamento de dados de temperatura, integridade estrutural e níveis de fluidos.
* **Lógica Go/No-Go:** Algoritmo de decisão automatizado para autorizar ou abortar o lançamento.
* **Simulação de Eventos:** Mini-game interativo que simula imprevistos espaciais (tempestades solares, vazamentos).
* **Cálculo Energético:** Avaliação de autonomia considerando perdas e consumo de decolagem.

## Dataset de Telemetria
O sistema utiliza um arquivo `.csv` contendo dados históricos de sensores para validar os sistemas.
> **[Clique aqui para baixar o dataset_telemetria_marte.csv](https://fiapcom-my.sharepoint.com/:x:/g/personal/rm571817_fiap_com_br/IQCnUwCybwgDQaX55Dr_xcrsAc_osW4fSnMfT-nfcdoB-rU?e=0Sok3j)**

## Tecnologias Utilizadas
* **Pandas:** Manipulação e análise de dados.
* **Google Colab API:** Interface para upload de arquivos em nuvem.
* **Random/Time:** Simulação de eventos aleatórios e latência de processamento.

## Como Executar no Google Colab
1.  Acesse o [Google Colab](https://colab.research.google.com/).
2.  Crie um novo Notebook e cole o código do arquivo principal.
3.  **Importante:** Ao iniciar a execução, o script solicitará o upload do arquivo de dados.
4.  Selecione o arquivo `dataset_telemetria_marte.csv` que você baixou.
5.  Interaja com o console para resolver os dilemas de missão (escolhas 1 ou 2).

## Funcionalidades do Script

### 1. Verificação de Segurança (Checklist)
O algoritmo valida se os parâmetros extraídos do dataset estão dentro das faixas seguras:
* **Temperatura Interna:** Entre 5°C e 40°C.
* **Integridade Estrutural:** Deve estar em 0 (sem danos detectados).
* **Energia e Combustível:** Mínimo de 100% para uma decolagem nominal segura.

### 2. Análise Energética
Cálculo automático de eficiência e viabilidade:
$Energia\ Real = (Capacidade \times Carga) - Perdas$

### 3. Evento de Dilema (Mini-game)
Durante a simulação, o sistema gera eventos aleatórios que testam a resiliência da missão:
* **Tempestade Solar:** Decida entre ativar escudos (gasta energia) ou confiar na blindagem.
* **Vazamento de O2:** Escolha entre selar setores ou enviar drones de reparo.

## Reflexão Ética e Sustentável
Este projeto integra conceitos de **ESG e responsabilidade socioambiental**. A gestão eficiente de energia na Aurora Siger reflete a necessidade de tecnologias que respeitem os limites de recursos, garantindo que a expansão interplanetária seja feita de forma ética e sustentável.

## Print da execução:
<img width="731" height="682" alt="image" src="https://github.com/user-attachments/assets/7672f563-aab3-4f5b-967f-fc57854009b5" />
<img width="752" height="471" alt="image" src="https://github.com/user-attachments/assets/2299ace3-4e13-4523-8d12-ce9f2d12d62a" />

---
## Desenvolvido como parte da Atividade Integradora - Fase 1
* **GABRIEL TAVARES MARTINS DE OLIVEIRA - RM573718**
* **MATHEUS HENRIQUE PEDROZO TRAIBA - RM571817**
* **PEDRO HENRIQUE DE LIMA COSTA - RM573008**