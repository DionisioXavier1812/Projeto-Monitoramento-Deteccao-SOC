# Threat Model — SOC Dio

## Visão Geral
Modelo de ameaças aplicado ao SOC Dio, cobrindo ingestão, correlação, detecção e resposta.

## Arquitetura
Fontes de Log ? Agentes ? Pipeline ? Normalização ? SIEM ? Regras ? Alertas ? Dashboards ? Resposta

## Ativos Críticos
- Servidores Dio  
- Aplicações Dio  
- Logs Dio  
- Credenciais  
- Dashboards  
- Pipelines  

## Ameaças
- Execução remota  
- Escalada de privilégios  
- Persistência  
- Exfiltração  
- Movimento lateral  

## Vetores de Ataque
- PowerShell  
- Serviços remotos  
- Credenciais válidas  
- Comunicação maliciosa  

## Controles Existentes
- Wazuh  
- Elastic  
- Sigma  
- Dashboards  
- Playbooks  

## Lacunas
- Falta de automação de resposta  
- Falta de correlação avançada  
- Falta de threat intelligence integrada  

## Recomendações
- Implementar SOAR  
- Integrar feeds de TI  
- Expandir regras Sigma  
