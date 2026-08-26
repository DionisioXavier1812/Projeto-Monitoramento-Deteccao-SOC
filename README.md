
# 🛡️ Projeto de Monitoramento e Detecção – SOC  
**Plataforma de Monitoramento, Correlação, Detecção e Resposta a Incidentes**

---

## 📌 Visão Geral

Este projeto tem como objetivo construir uma **plataforma completa de monitoramento e detecção**, alinhada às práticas de um **Security Operations Center (SOC)**.  
A solução abrange **coleta de logs**, **normalização**, **correlação**, **regras de detecção**, **alertas**, **dashboards**, e **playbooks de resposta**.

O foco é fornecer uma arquitetura modular, escalável e aplicável a ambientes reais, utilizando ferramentas open‑source e padrões amplamente adotados no mercado.

---

## 🎯 Objetivos do Projeto

- Criar uma estrutura SOC funcional para estudo, demonstração ou uso real.
- Implementar pipelines de ingestão de logs de múltiplas fontes.
- Desenvolver regras de detecção baseadas em MITRE ATT&CK.
- Criar dashboards para visualização de eventos e incidentes.
- Automatizar respostas com playbooks (opcional).
- Documentar arquitetura, casos de uso e fluxos de investigação.

---

## 🏗️ Arquitetura da Solução

A arquitetura proposta segue o fluxo:

```
[Fontes de Log]
    ↓
[Agentes de Coleta]
    ↓
[Pipeline de Ingestão]
    ↓
[Normalização e Enriquecimento]
    ↓
[SIEM / Motor de Correlação]
    ↓
[Regras de Detecção]
    ↓
[Alertas]
    ↓
[Dashboards]
    ↓
[Playbooks de Resposta]
```

### Tecnologias sugeridas
- **Wazuh / OSSEC** – Coleta e análise inicial  
- **Elastic Stack (ELK)** – SIEM, dashboards e correlação  
- **Sigma Rules** – Regras de detecção padronizadas  
- **Python / PowerShell** – Scripts auxiliares  
- **Docker Compose** – Ambiente replicável  

---

## 📂 Estrutura do Repositório

```
Projeto-Monitoramento-Deteccao-SOC/
│
├── README.md
├── docs/
│   ├── arquitetura.md
│   ├── casos_de_uso.md
│   ├── mitre_mapping.md
│   └── fluxo_investigacao.md
│
├── ingestion/
│   ├── agentes/
│   └── pipelines/
│
├── detections/
│   ├── sigma/
│   ├── elastic/
│   └── wazuh/
│
├── dashboards/
│   ├── kibana/
│   └── grafana/
│
├── response/
│   ├── playbooks/
│   └── scripts/
│
└── utils/
    ├── python/
    └── powershell/
```

---

## 🔍 Casos de Uso de Detecção

Alguns exemplos que serão implementados:

- Execução suspeita de PowerShell  
- Criação de usuários administrativos  
- Modificação de políticas de segurança  
- Execução de binários conhecidos por ataques (Living Off The Land)  
- Tentativas de brute force  
- Persistência via serviços  
- Comunicação com domínios maliciosos  

Cada caso de uso será mapeado à matriz **MITRE ATT&CK**.

---

## 🧠 Mapeamento MITRE ATT&CK

O projeto seguirá o framework MITRE para:

- Classificar técnicas e táticas detectadas  
- Criar regras de detecção alinhadas  
- Documentar gaps e oportunidades de melhoria  

Exemplo:

| Técnica | ID | Descrição | Detecção |
|--------|----|-----------|----------|
| PowerShell Execution | T1059.001 | Execução de comandos via PowerShell | Regras Sigma + Wazuh |

---

## 📊 Dashboards

Serão criados dashboards para:

- Eventos críticos  
- Autenticações  
- Atividades administrativas  
- Alertas correlacionados  
- Indicadores de ameaça (IOCs)  

Ferramentas sugeridas: **Kibana** e **Grafana**.

---

## 🚨 Alertas e Resposta

O projeto incluirá:

- Alertas automáticos via SIEM  
- Playbooks de resposta (manual e automatizada)  
- Scripts para coleta de evidências  
- Fluxos de investigação documentados  

---

## 🧪 Como Executar (quando implementado)

1. Instale Docker e Docker Compose  
2. Execute o ambiente:
   ```
   docker-compose up -d
   ```
3. Acesse o SIEM via navegador  
4. Configure agentes de coleta  
5. Importe dashboards e regras de detecção  

---

## 🤝 Contribuições

Contribuições são bem-vindas!  
Você pode:

- Criar novas regras de detecção  
- Adicionar dashboards  
- Documentar novos casos de uso  
- Melhorar pipelines de ingestão  

---

## 📜 Licença

Este projeto será licenciado sob **MIT License** (recomendado).  

---

