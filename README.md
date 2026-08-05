# 🎙️ AI Call Performance Analytics

Plataforma de auditoria inteligente de ligações desenvolvida para monitoramento de SDRs e equipes comerciais, utilizando Inteligência Artificial para transcrição, avaliação de qualidade, coaching automatizado e análise de performance operacional.

O projeto integra telefonia, banco de dados, automação de processos, IA Generativa e Power BI para transformar chamadas comerciais em insights acionáveis para gestores.

> **Status: em produção desde julho/2026.** A solução operou primeiro em ambiente de homologação (n8n local + PostgreSQL) e hoje roda 100% em produção, de forma agendada e autônoma, sobre **n8n Cloud** e **MySQL**.

## 🚀 Objetivo

Permitir que gestores acompanhem a qualidade das ligações realizadas pela equipe comercial sem a necessidade de ouvir manualmente centenas de gravações.

A solução automatiza:

* Captura de chamadas da API4Com
* Armazenamento estruturado em banco relacional (MySQL, em produção)
* Transcrição automática de áudio
* Avaliação de qualidade com IA
* Feedback individual para SDRs
* Relatórios consolidados de coaching
* Dashboards gerenciais em Power BI, atualizados 8x ao dia

## 🏗️ Arquitetura da Solução

```
API4Com
    ↓
n8n Cloud
    ↓
MySQL
    ↓
OpenAI Whisper
    ↓
GPT-4o-mini
    ↓
Power BI
```

### Componentes

* API4Com
* n8n Cloud
* MySQL
* OpenAI Whisper
* GPT-4o-mini
* Power BI
* Node.js

## 🤖 Recursos de Inteligência Artificial

### Transcrição Automática
As gravações são processadas automaticamente através do OpenAI Whisper para conversão de áudio em texto.

### Avaliação de Ligações
Cada chamada pode receber:

* Nota de qualidade (0 a 10)
* Resumo da conversa
* Feedback individual
* Pontos de melhoria

### Coaching Comercial
O sistema consolida múltiplas chamadas e gera:

* Nota geral do atendente
* Pontos fortes
* Pontos de melhoria
* Feedback consolidado

### Dialing Gap
Métrica de cadência de discagem: mede o intervalo entre o fim de uma chamada e o início da próxima, identificando tempo de preparação ideal por SDR, zonas de ociosidade e permitindo comparar ritmo entre membros do time.

### Inteligência Geoespacial
Heatmap de efetividade cruzando dia da semana e horário para identificar as melhores janelas de discagem, além de diagnóstico da qualidade da base de leads (números inválidos vs. atendidos).

## 📊 Dashboard Geral

Visão executiva da operação comercial.

### Indicadores

* Total de ligações
* Ligações atendidas
* Ligações efetivas
* Taxa de conversão
* Tempo médio de atendimento
* Custo operacional
* Custo por ligação efetiva

## 📞 Monitoramento de Ligações

Consulta detalhada de chamadas realizadas.

### Informações Disponíveis

* Data da ligação
* Atendente
* Ramal
* Número de destino
* Status da chamada
* Duração
* Custo
* Link da gravação

## 👥 Performance da Equipe

Painel comparativo para acompanhamento da produtividade dos atendentes.

### Métricas

* Ligações realizadas
* Conversão
* Efetividade
* Tempo falado
* Custo operacional
* Taxa de recontato

## 🧠 Auditoria Inteligente de Ligações

A IA analisa individualmente as chamadas e gera avaliações automáticas.

### Recursos

* Nota da ligação
* Resumo automático
* Feedback contextual
* Histórico de análises

## 📈 Coaching de SDRs

Visão consolidada das últimas ligações analisadas para acompanhamento contínuo da evolução do profissional.

### Entregas

* Resumo diário
* Feedback consolidado
* Evolução da performance
* Recomendações práticas

## 📌 Resultados Obtidos

Durante a validação da solução foram processadas:

* Mais de 28.000 chamadas
* Centenas de transcrições automáticas
* Auditorias individuais geradas por IA
* Relatórios consolidados de coaching
* Integração com telefonia e CRM

Em produção, o sistema roda de forma contínua e agendada (sem gatilho manual), com cobertura de 100% das chamadas qualificadas (≥ 60 segundos).

## 💰 Viabilidade Financeira

Além dos ganhos operacionais, o projeto inclui uma análise de custos e retorno sobre investimento (ROI) para validar a utilização da Inteligência Artificial em larga escala — validada com dados reais de uma semana completa de operação em produção.

### Benefícios Financeiros

* Auditoria automática de 100% das chamadas qualificadas.
* Redução superior a 95% dos custos em comparação ao modelo tradicional de auditoria manual.
* Custo médio real de aproximadamente **R$ 26,55/dia útil** (OpenAI) em produção, projetando um custo mensal total (OpenAI + n8n Cloud) de **~R$ 618,92/mês**.
* Escalabilidade sem necessidade de ampliação proporcional da equipe de monitoria.
* Feedback imediato para gestores e SDRs, acelerando ciclos de melhoria contínua.

### Impacto no Negócio

A solução transforma um processo tradicionalmente manual e amostral em uma operação escalável, permitindo monitorar integralmente a qualidade dos atendimentos com baixo custo operacional e alto potencial de retorno para áreas comerciais e de atendimento.

## 🛠️ Tecnologias Utilizadas

* Power BI
* MySQL
* n8n Cloud
* OpenAI Whisper
* GPT-4o-mini
* Node.js
* API4Com
* SQL
* Inteligência Artificial Generativa

## 👨‍💼 Autor

**Paulo Henrique Miranda**
Analista de Projetos com experiência em:

* CRM
* Power BI
* Automação de Processos
* Inteligência Artificial
* Integração de APIs
* Analytics

📎 LinkedIn: https://www.linkedin.com/in/pmirandabh/
📎 GitHub: https://github.com/pmirandabh
