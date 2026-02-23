# 📅 Cronograma Detalhado: Smart Badge - Detector de Quedas (LARAF 2026)

Este documento detalha o planejamento das **18 semanas de desenvolvimento do Smart Badge**, um crachá inteligente projetado para detectar quedas em idosos e acionar resgate imediato via Wi-Fi.

---

## 🏗️ Divisão de Responsabilidades (Squads)

### **P1 (Requisitos e UX)**
- Mapeamento de stakeholders  
- Jornada do usuário  
- Interface do App/Portal  

### **P2 (Arquitetura e Firmware)**
- Lógica do MPU6050  
- Algoritmos de detecção de queda  
- Integração com Backend  

### **P3 (Hardware e Materiais)**
- Especificação de BOM  
- Gerenciamento de bateria (18650 + TP4056)  
- Montagem física  

---

# 🗓️ Fase 1: Imersão Técnica (Semanas 1 - 4)

**Objetivo:** Alinhamento de escopo e validação dos sensores de movimento.

| Semana | Atividade | Detalhamento Técnico |
|--------|-----------|----------------------|
01 | Kickoff e Foco | Estudo do escopo; Definição de metas do MVP; Alinhamento entre os squads P1, P2 e P3 |
02 | Workshop: ESP32 | Mapeamento de requisitos de hardware; Configuração do ambiente de desenvolvimento (Arduino IDE / PlatformIO) |
03 | Workshop: MPU6050 | Testes de leitura do acelerômetro e giroscópio; Estudo da biblioteca Adafruit MPU6050; Definição da arquitetura de dados |
04 | Unboxing e Bancada | Chegada dos materiais; Teste de carga/descarga da bateria 18650 com o módulo TP4056; Validação do BOM |

---

# 🚀 Fase 2: Desenvolvimento MVP (Semanas 5 - 8)

**Objetivo:** Criar o algoritmo de detecção e a infraestrutura de rede.

| Semana | Atividade | Detalhamento Técnico |
|--------|-----------|----------------------|
05 | Sprint Lógica Base | Desenvolvimento do algoritmo de queda (análise de vetores G); Diferenciação entre tropeço e queda com imobilidade |
06 | Sprint Conectividade | Criação do Portal/App para cadastro; Implementação do pareamento via Wi-Fi; Interface inicial |
07 | Integração de HW | Integração total: ESP32 + MPU6050 + Buzzer; Autenticação segura com Banco de Dados |
08 | Validação de Bancada | Implementação de telemetria e logs; Pipeline de dados para monitoramento em tempo real |

---

# 🛠️ Fase 3: Refinamento e Case (Semanas 9 - 12)

**Objetivo:** Otimização do sistema e construção do protótipo vestível.

| Semana | Atividade | Detalhamento Técnico |
|--------|-----------|----------------------|
09 | Estabilidade (QA) | Redução do consumo de energia (Deep Sleep no ESP32); Correção de bugs de conexão |
10 | Montagem End-to-End | Testes integrando hardware final com o App; Verificação do tempo de resposta do buzzer |
11 | Teste em Campo I | Testes controlados em ambiente real; Calibração de sensibilidade para evitar falsos positivos |
12 | Teste de Segurança | Hardening; Testes de OTA (Over The Air) e confiabilidade do sistema |

---

# 📊 Fase 4: Coleta de Dados e Entrega (Semanas 13 - 18)

**Objetivo:** Testes com usuários finais e documentação oficial.

| Semana | Atividade | Detalhamento Técnico |
|--------|-----------|----------------------|
13 | Geração de Métricas | Homologação interna; Checklist de critérios de entrega (DoD); Coleta de latência de rede |
14 | Piloto com Usuários | Testes de usabilidade com idosos/cuidadores; Feedback sobre conforto do crachá |
15 | Relatório Técnico | Finalização do documento de arquitetura; Ajustes finais no código |
16 | Manual do Usuário | Guia de operação, carregamento da bateria e configuração do App |
17 | Preparação Final | Ensaio da apresentação; Ajustes estéticos; Preparação do rollout |
18 | Entrega do MVP | Apresentação final e entrega do protótipo funcional ao LARAF |

---

# ✅ Definição de Pronto (DoD)

- O algoritmo deve diferenciar **quedas reais de movimentos bruscos cotidianos**
- O alerta sonoro deve ser **cancelável pelo usuário antes do envio via Wi-Fi**
- A bateria deve suportar **no mínimo 12 horas de monitoramento contínuo**

---
