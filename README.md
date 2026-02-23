# Smart Badge: Detector de Quedas e Resgate Imediato (LARAF 2026)

**Status do Projeto:** 🛠️ Em Desenvolvimento  
**Fase Atual:** Imersão Técnica

---

## 📝 Sobre o Projeto

O **Smart Badge** é um crachá inteligente projetado para aumentar a segurança de idosos e pessoas em grupos de risco.

O dispositivo utiliza sensores de movimento para detectar quedas automaticamente e, em caso de emergência:

- 🔊 Aciona um alarme sonoro local  
- 🌐 Envia notificações imediatas via Wi-Fi para cuidadores ou equipes de resgate  

---

## ⚠️ O Problema

Cerca de **30% a 50% dos idosos sofrem quedas anualmente**.

A demora no socorro pode:

- Agravar fraturas e traumas  
- Causar complicações médicas  
- Gerar impactos psicológicos (ansiedade e medo de viver sozinho)  

---

## ✅ A Solução

Um dispositivo **vestível (wearable) de baixo custo** que:

- Monitora aceleração e inclinação em tempo real  
- Diferencia movimentos bruscos de quedas reais  
- Emite alerta sonoro local com buzzer  
- Notifica uma central ou aplicativo via internet  

---

## 🚀 Tecnologias Utilizadas

### 🔌 Hardware

- **Microcontrolador:** ESP32 NodeMCU (Wi-Fi/Bluetooth e baixo consumo)
- **Sensor de Movimento:** MPU6050 (acelerômetro + giroscópio)
- **Gestão de Energia:**  
  - Bateria Li-ion 18650  
  - Módulo de carga TP4056
- **Interface:**  
  - Buzzer ativo  
  - Botões de pânico / reset  

### 💻 Software & Protocolos

- **Firmware:** C++ (Arduino IDE / PlatformIO)
- **Algoritmo:**  
  - Filtro complementar  
  - Análise de vetores de força G
- **Integração:**  
  - Web Portal  
  - Dashboard de monitoramento  

---

## 📅 Cronograma de Desenvolvimento

O projeto está dividido em **4 fases principais**:

### 🔹 Fase 1 — Imersão Técnica (Semanas 1–4)
- Estudos de hardware  
- Workshop do MPU6050  
- Unboxing de materiais  

### 🔹 Fase 2 — Desenvolvimento do MVP (Semanas 5–8)
- Algoritmo de detecção de quedas  
- Integração com portal web  

### 🔹 Fase 3 — Refinamento e Case (Semanas 9–12)
- Deep Sleep para economia de bateria  
- Redução do tamanho do dispositivo  
- Testes de segurança  

### 🔹 Fase 4 — Coleta de Dados e Entrega (Semanas 13–18)
- Testes com usuários reais  
- Coleta de métricas  
- Entrega do protótipo final  

📌 Para o planejamento completo, consulte o **Cronograma Detalhado**.

---

## 👥 Organização da Equipe (Squads)

### 🧩 Squad P1 — Requisitos & UX
- Jornada do usuário  
- Interface do aplicativo  

### ⚙️ Squad P2 — Firmware & Lógica
- Código de detecção de quedas  
- Processamento de dados  

### 🔩 Squad P3 — Hardware & Case
- Eletrônica  
- Bateria  
- Design físico do crachá  

---

## 🔧 Como Contribuir

```bash
# Clone o repositório
git clone https://github.com/seu-usuario/smart-badge.git
