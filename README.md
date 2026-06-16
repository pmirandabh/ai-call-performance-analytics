# 🎙️ AI Call Performance Analytics

Plataforma de auditoria inteligente de ligações desenvolvida para monitoramento de SDRs e equipes comerciais, utilizando Inteligência Artificial para transcrição, avaliação de qualidade, coaching automatizado e análise de performance operacional.

O projeto integra telefonia, banco de dados, automação de processos, IA Generativa e Power BI para transformar chamadas comerciais em insights acionáveis para gestores.

---

## 🚀 Objetivo

Permitir que gestores acompanhem a qualidade das ligações realizadas pela equipe comercial sem a necessidade de ouvir manualmente centenas de gravações.

A solução automatiza:

- Captura de chamadas da API4Com
- Armazenamento estruturado em PostgreSQL
- Transcrição automática de áudio
- Avaliação de qualidade com IA
- Feedback individual para SDRs
- Relatórios consolidados de coaching
- Dashboards gerenciais em Power BI

---

## 🏗️ Arquitetura da Solução

```text
API4Com
    ↓
n8n
    ↓
PostgreSQL
    ↓
OpenAI Whisper
    ↓
GPT-4o-mini
    ↓
Power BI
```

### Componentes

- API4Com
- n8n
- PostgreSQL
- OpenAI Whisper
- GPT-4o-mini
- Power BI
- Node.js

---

## 🤖 Recursos de Inteligência Artificial

### Transcrição Automática

As gravações são processadas automaticamente através do OpenAI Whisper para conversão de áudio em texto.

### Avaliação de Ligações

Cada chamada pode receber:

- Nota de qualidade
- Resumo da conversa
- Feedback individual
- Pontos de melhoria

### Coaching Comercial

O sistema consolida múltiplas chamadas e gera:

- Nota geral do atendente
- Pontos fortes
- Pontos de melhoria
- Feedback consolidado

---

## 📊 Dashboard Geral

Visão executiva da operação comercial.

### Indicadores

- Total de ligações
- Ligações atendidas
- Ligações efetivas
- Taxa de conversão
- Tempo médio de atendimento
- Custo operacional
- Custo por ligação efetiva

![Dashboard Geral](Tela%20Geral.png)

---

## 📞 Monitoramento de Ligações

Consulta detalhada de chamadas realizadas.

### Informações Disponíveis

- Data da ligação
- Atendente
- Ramal
- Número de destino
- Status da chamada
- Duração
- Custo
- Link da gravação

![Dashboard Ligações](Tela%20das%20Ligações.png)

---

## 👥 Performance da Equipe

Painel comparativo para acompanhamento da produtividade dos atendentes.

### Métricas

- Ligações realizadas
- Conversão
- Efetividade
- Tempo falado
- Custo operacional
- Taxa de recontato

![Dashboard Equipe](Tela%20do%20resultado%20da%20Equipe.png)

---

## 🧠 Auditoria Inteligente de Ligações

A IA analisa individualmente as chamadas e gera avaliações automáticas.

### Recursos

- Nota da ligação
- Resumo automático
- Feedback contextual
- Histórico de análises

![Análise IA](Tela%20de%20Analise%20individual%20da%20Ligação.png)

---

## 📈 Coaching de SDRs

Visão consolidada das últimas ligações analisadas para acompanhamento contínuo da evolução do profissional.

### Entregas

- Resumo diário
- Feedback consolidado
- Evolução da performance
- Recomendações práticas

![Coaching IA](Tela%20da%20Analise%20do%20Atendente.png)

---

## 📌 Resultados Obtidos

Durante a validação da solução foram processadas:

- Mais de 28.000 chamadas
- Centenas de transcrições automáticas
- Auditorias individuais geradas por IA
- Relatórios consolidados de coaching
- Integração com telefonia e CRM

---
## 💰 Viabilidade Financeira

Além dos ganhos operacionais, o projeto inclui uma análise de custos e retorno sobre investimento (ROI) para validar a utilização da Inteligência Artificial em larga escala.

### Benefícios Financeiros

* Auditoria automática de 100% das chamadas qualificadas.
* Redução superior a 95% dos custos em comparação ao modelo tradicional de auditoria manual.
* Custo médio aproximado de R$ 0,11 por chamada auditada.
* Escalabilidade sem necessidade de ampliação proporcional da equipe de monitoria.
* Feedback imediato para gestores e SDRs, acelerando ciclos de melhoria contínua.

### Impacto no Negócio

A solução transforma um processo tradicionalmente manual e amostral em uma operação escalável, permitindo monitorar integralmente a qualidade dos atendimentos com baixo custo operacional e alto potencial de retorno para áreas comerciais e de atendimento.

## 🛠️ Tecnologias Utilizadas

- Power BI
- PostgreSQL
- n8n
- OpenAI Whisper
- GPT-4o-mini
- Node.js
- API4Com
- SQL
- Inteligência Artificial Generativa

---

## 👨‍💼 Autor

### Paulo Henrique Miranda

Analista de Projetos com experiência em:

- CRM
- Power BI
- Automação de Processos
- Inteligência Artificial
- Integração de APIs
- Analytics

📎 LinkedIn:
https://www.linkedin.com/in/pmirandabh/

📎 GitHub:
https://github.com/pmirandabh
