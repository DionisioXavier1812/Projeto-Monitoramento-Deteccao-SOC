# Threat Model — Projeto-Monitoramento-Deteccao-SOC

## ?? Objetivo
Modelar ameaças, superfícies de ataque, vetores, técnicas MITRE e impactos no ambiente SOC simulado.

## ??? Arquitetura
- AD Domain Controller
- Servidor de Aplicações
- Estações Windows
- Firewall + IDS
- Servidor de Logs (SIEM)

## ?? Vetores de Ataque
- PowerShell malicioso
- Credential Harvesting
- Exfiltração HTTPS
- Movimento lateral
- Persistência

## ?? MITRE ATT&CK Mapping
- T1059 — Command Execution
- T1003 — Credential Dumping
- T1041 — Exfiltration over HTTPS
- T1021 — Lateral Movement
- T1053 — Scheduled Tasks (Persistence)

## ?? Superfícies de Ataque
- Credenciais fracas
- Falhas de hardening
- Logs insuficientes
- Exposição de serviços

## ??? Controles Recomendados
- Hardening AD
- PowerShell Constrained Language Mode
- Sysmon + Sigma
- MFA
- Network Segmentation
