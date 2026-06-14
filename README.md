# AtmoSense Web: Simulador e Documentação Interativa 🌱

Bem-vindo ao portal interativo do **AtmoSense**. 

Este repositório contém a aplicação web Front-end cujo objetivo principal é **documentar a arquitetura** do projeto original e **simular em tempo real** a tomada de decisão do nosso motor de inteligência agrometeorológica.

> ⚠️ **Nota Importante:** Este repositório diz respeito **apenas à interface de simulação web**. O código-fonte dos hardwares IoT (nós de campo), sistemas embarcados e serviços de backend que executam no mundo real estão localizados em repositórios separados.

## 🎯 Objetivo Deste Portal

O sistema físico do AtmoSense é complexo e atua silenciosamente no campo. Desenvolvemos este portal conceitual para materializar a lógica do sistema e permitir que desenvolvedores, agrônomos e investidores possam **visualizar matematicamente** como o AtmoSense economiza recursos hídricos.

Em vez de testar diretamente em uma fazenda, você pode usar este site para injetar dados meteorológicos simulados e ver como os algoritmos reagem na estufa ou no campo aberto.

## 🗺️ Estrutura da Plataforma

A aplicação está dividida em três pilares principais de exploração:

### 1. 📊 Dashboard (Simulador)
Um ambiente sandbox (`SimuladorView.tsx`) que imita o painel de controle real do AtmoSense.
* **Previsão vs Consumo Real:** Compara curvas de Evapotranspiração da cultura contra o balanço hídrico das chuvas.
* **Motor de Regras:** Demonstra o processamento matemático em tempo real do Ponto de Orvalho (risco de fungos) e do VPD (Déficit de Pressão de Vapor).
* **Console de Telemetria:** Um log interativo detalhando os cálculos vetoriais e decisões que estão sendo tomadas pelas fórmulas em plano de fundo.

### 2. 🧠 Conceito e Lógica (Scientific Logic)
Uma seção puramente explicativa detalhando as fórmulas por trás do produto. Traduzimos conceitos de alto nível da agronomia global (FAO-56) e termodinâmica foliar para uma linguagem visual e compreensível, mostrando o *porquê* da regra clássica de rega estar obsoleta frente a algoritmos dinâmicos.

### 3. 🏗️ Arquitetura Técnica
A documentação visual da engenharia do projeto. Mapeia como os microcontroladores de campo, sensores de umidade, estações de previsão (como INMET) e a inteligência em nuvem conversam entre si para formar o robusto ecossistema físico do AtmoSense.

## 🛠️ Stack Tecnológico do Simulador

Como este projeto foca em alta reatividade, clareza em visualização de dados e performance para cálculos simulados na web, utilizamos:

* **React 18 + Vite:** Renderização de alta performance.
* **Tailwind CSS:** Para interfaces modernas, responsivas e limpas.
* **Chart.js / React-Chartjs-2:** Para a renderização das curvas de balanço hídrico, simulações termodinâmicas e gráficos.
* **Lucide React:** Iconografia padronizada e polida.

## 🚀 Como Rodar o Simulador Localmente

Se você deseja explorar a lógica, mexer nos parâmetros de simulação ou testar diferentes cenários agronômicos:

1. Clone este repositório simulador:
   ```bash
   git clone https://github.com/seu-usuario/atmosense-simulador-web.git
