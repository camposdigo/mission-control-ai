# Mission Control AI

### Mobile Predictive Monitoring & Mission Operations Dashboard

![Mission Control AI](./assets/screenshots/banner.png)

Aplicativo mobile desenvolvido com **React Native, Expo e TypeScript** para monitoramento de uma missão orbital simulada. A solução centraliza telemetria, energia, comunicação e estabilidade operacional em dashboards e gera alertas automaticamente a partir de limites configuráveis.

> **Problema:** ambientes operacionais complexos geram muitos indicadores simultâneos, dificultando a identificação rápida de condições críticas.
>
> **Solução:** o Mission Control AI transforma diferentes sinais operacionais em dashboards, indicadores de risco, alertas e recomendações em uma interface mobile centralizada.

## Visão do produto

```text
Sensores + Energia + Comunicação + Órbita
                    ↓
             Estado global
                    ↓
          Regras e limiares
                    ↓
       Dashboards + Alertas
                    ↓
       Resposta operacional
```

## Principais funcionalidades

- Dashboard executivo da missão
- Readiness score e probabilidade simulada de falha
- Monitoramento de sensores e temperatura
- Monitoramento de bateria e entrada solar
- Qualidade de comunicação e latência
- Indicadores de estabilidade orbital
- Alertas automáticos baseados em limiares configuráveis
- Timeline de incidentes e recomendações
- Persistência das configurações no dispositivo
- Simulação de incidentes operacionais
- Console inspirado no Apollo Guidance Computer

## Interface

### Dashboard principal

![Home](./assets/screenshots/home.png)

Visão consolidada da saúde operacional, readiness score, probabilidade de falha, alertas ativos e ação recomendada.

### Mapa orbital

![Mapa orbital](./assets/screenshots/home-mapa.png)

Representação da nave, estabilidade, deriva e estado dos subsistemas.

### Telemetria

![Telemetria](./assets/screenshots/telemetria.png)

Dashboard para acompanhamento dos indicadores simulados da missão.

### Comunicação

![Comunicação](./assets/screenshots/telemetria-comunicacao.png)

Qualidade do link, sinal, latência e estabilidade operacional.

### Resposta a incidentes

![Alertas](./assets/screenshots/resposta.png)

Alertas são produzidos automaticamente quando os dados ultrapassam os limites definidos pelo operador.

### Timeline operacional

![Timeline](./assets/screenshots/resposta-timeline.png)

Histórico de eventos detectados, recomendações e parâmetros utilizados pelo sistema.

### Configuração de limites

![Configurações](./assets/screenshots/configuracoes-limiares.png)

Permite configurar limites de temperatura, bateria, sinal, latência e estabilidade, com persistência local.

### Apollo Guidance Computer

![AGC](./assets/screenshots/agc.png)

Console inspirado no AGC com programas, registradores, comandos e alarmes simulados.

## Arquitetura e engenharia

O projeto utiliza gerenciamento de estado compartilhado para manter os diferentes dashboards sincronizados.

- **Context API** para distribuição do estado
- **useReducer** para gerenciamento centralizado da missão
- **useState / useEffect** para interface, formulários e simulação
- **AsyncStorage** para persistência local
- **Expo Router** para navegação
- componentes reutilizáveis
- TypeScript para tipagem e manutenção do código

## Tecnologias

- React Native
- Expo SDK 54
- TypeScript
- Expo Router
- Context API
- AsyncStorage
- React Native Reanimated
- React Native Screens
- React Native Safe Area Context

## O que este projeto demonstra

Além do cenário espacial, a arquitetura representa padrões aplicáveis a sistemas reais de monitoramento:

- dashboards operacionais
- acompanhamento de KPIs em tempo real
- sistemas de alertas
- aplicativos de monitoramento IoT
- painéis de infraestrutura
- acompanhamento de equipamentos e sensores
- interfaces para operações críticas

## Como executar

```bash
git clone https://github.com/camposdigo/GS-CPAD.git
cd GS-CPAD
npm install
npm run start:lan
```

Abra o projeto utilizando Expo Go em um dispositivo compatível com Expo SDK 54.

## Demonstração

O repositório inclui screenshots das principais telas em `assets/screenshots/`.

Também existe uma demonstração em vídeo do projeto disponível na documentação original do trabalho.

## Contexto

Projeto desenvolvido originalmente para a **Global Solution 2026.1 — Cross-Platform Application Development | FIAP**, no desafio *Space Predictive Analytics*.

A apresentação deste repositório destaca também os conceitos de arquitetura, monitoramento e desenvolvimento mobile que podem ser reutilizados em aplicações comerciais.

## Autor

**Rodrigo Campos Cordeiro — RM566386**

Mobile Development • Dashboards • TypeScript • React Native
