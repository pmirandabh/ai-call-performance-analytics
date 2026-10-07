# 🎙️ AI Call Performance Analytics

Plataforma de auditoria inteligente de ligações para equipes comerciais. Usa Inteligência Artificial para transcrever chamadas, avaliar a qualidade de cada uma e gerar coaching automático para SDRs, com dashboards para gestores.

> **Aviso:** este repositório documenta a solução. Dados de clientes, valores e informações internas da empresa foram removidos ou mascarados nas imagens.

**Status:** em produção, de forma agendada e autônoma (n8n Cloud + MySQL). Antes disso, a solução foi validada em ambiente de homologação.

## 🎯 O problema

Gestores comerciais conseguem ouvir só uma pequena fração das ligações da equipe. O feedback demora, depende da percepção de cada pessoa e o critério muda de auditor para auditor.

## 🚀 A solução

Uma esteira automática que:

- captura as ligações direto da telefonia (API4Com);
- separa as chamadas qualificadas (a partir de 60 segundos);
- transcreve o áudio;
- avalia cada ligação com IA, com nota, resumo e feedback;
- consolida o desempenho de cada atendente (diário, semanal e mensal);
- entrega tudo em dashboards no Power BI.

## 🏗️ Arquitetura

```
API4Com (telefonia)
        ↓
   n8n Cloud (orquestração)
        ↓
      MySQL
        ↓
 OpenAI Whisper (transcrição)
        ↓
 GPT-4o-mini (avaliação)
        ↓
     Power BI
```

**Componentes:** API4Com, n8n Cloud, MySQL, OpenAI Whisper, GPT-4o-mini, Power BI, Node.js, SQL.

## 🤖 Recursos de IA

- **Transcrição automática** das gravações.
- **Avaliação por ligação:** nota de 0 a 10, resumo da conversa, feedback individual e pontos de melhoria.
- **Coaching consolidado:** nota geral do atendente, pontos fortes, pontos de melhoria e feedback do período.
- **Tratamento de casos especiais**, como ligações que caem em caixa postal, que não devem receber nota de atendimento.

## 📊 Análises no Power BI

- **Visão geral:** volume, ligações atendidas e efetivas, taxa de conversão e tempo médio.
- **Performance da equipe:** comparação de produtividade entre atendentes.
- **Dialing Gap:** intervalo entre o fim de uma chamada e o início da próxima, para identificar ociosidade e ritmo de cada SDR.
- **Heatmap de efetividade:** dia da semana e horário, para achar as melhores janelas de discagem e avaliar a qualidade da base de leads.
- **Auditoria de ligações:** nota, resumo, feedback e histórico de cada chamada.

## 🧩 Decisões de projeto

- **Triagem antes da IA.** Nem toda ligação merece análise. Uma regra de triagem separa o que vale a pena avaliar do que é ruído, antes de qualquer chamada de API. Isso reduziu o custo de processamento de IA em cerca de 85%, sem perder chamadas relevantes.
- **Automação 100% agendada**, sem gatilho manual, com tentativas automáticas em caso de falha.
- **Critério único de avaliação.** O mesmo padrão é aplicado a todas as ligações, o que elimina a variação entre auditores.
- **Feedback no mesmo dia**, em vez de dias depois.

## 📌 Resultados

- Cobertura de 100% das ligações qualificadas, de forma contínua.
- Dezenas de milhares de chamadas processadas na validação.
- Feedback disponível no mesmo dia da ligação.
- Fim da auditoria manual por amostragem.

## 💰 Viabilidade financeira

O projeto inclui um modelo de custo por ligação analisada (transcrição mais avaliação por IA), comparado ao custo de uma auditoria manual por amostragem. Na validação, o custo da IA por ligação ficou em uma fração do custo da auditoria humana, o que viabiliza cobrir todas as chamadas qualificadas. Os valores absolutos são internos e não são publicados aqui.

## 📚 Aprendizados

- Orquestração de fluxos complexos no n8n.
- Engenharia de prompts e controle de qualidade das respostas da IA.
- Otimização de custo em aplicações com LLM.
- Modelagem de dados para análise de performance e BI.
- Transformar um processo manual e amostral em operação contínua e mensurável.

## 🛠️ Tecnologias

Power BI · MySQL · n8n Cloud · OpenAI Whisper · GPT-4o-mini · Node.js · API4Com · SQL

## 👨‍💼 Autor

**Paulo Henrique Miranda**, RevOps & AI Automation. CRM, Power BI, automação de processos e IA aplicada a vendas.

📎 [LinkedIn](https://www.linkedin.com/in/pmirandabh/)
