# 🚀 Sistema de Gestão e Automação - ONG Vida Plena


## 📖 Sobre o Projeto
Este projeto consiste na modelagem e implementação de um **Sistema de Gerenciamento de Dados Relacional** para a ONG fictícia "Vida Plena".

O objetivo foi solucionar a desorganização de dados (planilhas descentralizadas e grupos de WhatsApp) criando uma aplicação **No-Code** centralizada, segura e automatizada. O sistema permite o cadastro de beneficiários, gestão de eventos e controle de histórico de participações, com foco em **Business Intelligence (BI)** e conformidade com a **LGPD**.

---

## ⚙️ Funcionalidades Principais

### 1. Modelagem de Dados Relacional
Estruturação de um banco de dados robusto com relacionamento **Muitos-para-Muitos (N:M)**:
* **Beneficiários:** Cadastro único (evita duplicidade).
* **Eventos:** Agenda de atividades da ONG.
* **Inscrições (Tabela Associativa):** Vincula pessoas a eventos, gerando histórico.

### 2. Automação de Processos
* **Integração Airtable + Gmail:** Disparo automático de e-mails de confirmação contendo Data e Local assim que o formulário de inscrição é enviado.
* **Notificações Administrativas:** Alerta para a gestão a cada nova movimentação.

### 3. Interfaces e UX
* **Formulários Web:** Interfaces simplificadas para voluntários (input de dados) sem acesso à base bruta.
* **Dashboard Gerencial:** Visualização de Total de Atendimentos e Calendário de Eventos em tempo real.

### 4. Lógica Avançada
* **Override de Datas:** Implementação de campo calculado (Fórmula) que gerencia datas automáticas (*timestamp*) para novos registros, mas permite inserção manual para cargas históricas de eventos passados.

---

## 🛠️ Tecnologias Utilizadas

* **Airtable:** Banco de Dados Relacional e Interface.
* **Gmail Integration:** Automação de e-mail transacional.
* **Miro:** Levantamento de requisitos e Brainstorming.
* **brModelo:** Modelagem Conceitual e Lógica (DER).
* **4Devs:** Geração de dados reais para testes.

---

## 🔒 Segurança e LGPD (Privacidade)

O projeto foi desenvolvido seguindo os princípios da Lei Geral de Proteção de Dados:

* **Minimização de Dados:** Coleta de **Idade** justificada para fins de adequação pedagógica dos eventos.
* **Dados Opcionais:** Campos como **Foto** e **Endereço** são opcionais, focados apenas na humanização e geolocalização, respeitando o consentimento do titular.
* **Controle de Acesso:** Voluntários operam apenas via Formulários; Gestores acessam Dashboards. Visitantes somente visualizam.

---

## 📸 Demonstração Visual

### Modelo Relacional (Diagrama)
*(Espaço para colocar os prints dos diagramas brModelo e Miro)*



### Dashboard de Gestão
*(Espaço para colocar o print da sua Interface do Airtable)*
`[Insira sua imagem aqui]`

---

## 🚀 Como Executar/Reproduzir

Como este é um projeto No-Code hospedado em nuvem:

1.  O acesso ao sistema é feito via **Airtable**.
2.  Os fluxos de entrada de dados ocorrem via **Formulários Públicos**.
3.  A lógica de automação roda no servidor do Airtable (Trigger: *When record is created* > Action: *Send Email via Gmail*).

https://airtable.com/invite/l?inviteId=invmIg6THqz8PFJhF&inviteToken=3dd3237bcf9bcef03a214c442999f5870d176bb520d9a22036b347dd4c66b6bc&utm_medium=email&utm_source=product_team&utm_content=transactional-alerts

---

## 👩‍💻 Autora

**Gabi**
*Estudante de IA e Automação Digital | Bacharel em Direito | Escrevente e Encarregada de Dados*


