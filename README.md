#  Agente de IA para Automação de Monitoria de Qualidade

> Automação inteligente desenvolvida para realizar análises e monitorias de qualidade automatizadas a partir de transcrições de atendimentos, otimizando o fluxo de QA e a extração de indicadores operacionais.

---

##  Objetivo & Contexto de Negócio

* **Problema:** A equipe de qualidade realizava 100% das monitorias de forma manual. Cada análise de atendimento levava em média de 15 a 20 minutos, gerando um gargalo operacional e limitando a cobertura de auditoria do time.
* **Solução:** Implementação de um **Agente de IA no Zapier** integrado à API da OpenAI. A automação extrai as transcrições dos atendimentos diretamente de uma planilha, executa a análise de qualidade completa de forma autônoma e devolve a monitoria concluída na própria planilha. Além da auditoria de qualidade, a solução foi expandida para analisar outros indicadores estratégicos de negócio, como precificação, descartes e conformidade de processos.

---

## Ferramentas

* **Orquestração & Fluxo:** [Zapier](Webhooks, Google Sheets / Excel, Paths)
* **Inteligência Artificial:** OpenAI API (`gpt-4o` / ChatGPT)
* **Integrações de Destino:** Google Sheets / Microsoft Excel, E-mail / Google Chat
* **Lógica Extra:** Javascript / Python (via *Code by Zapier* para tratamento e formatação de payloads)

---

## Demonstração Visual

### 1. Fluxo da Automação no Zapier
![Fluxo do Zapier](

https://github.com/user-attachments/assets/5363a754-c921-421b-a58d-3c2803432cf5

)

### 2. Planilha de Resultados (Monitoria Concluída & Indicadores)
![Planilha de Monitorias](resultadomonitoria.png)

---

##  Arquitetura do Fluxo
[ Gatilho: Nova Transcrição na Planilha ]
│
▼
[ Zapier: Format & Clean Data ]
│
▼
[ Chamada OpenAI API / Prompt QA ]
(Análise de Qualidade, Precificação e Descartes)
│
▼
[ Retorno dos Dados Auditados na Planilha ]
│
▼
[ Alerta / Notificação de Conclusão ]
