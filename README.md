# Projeto Microsoft 365 Admin: LAB-A02 
**Administrador:** José Lucas Cainda  

Este repositório contém a documentação técnica e os relatórios de execução das fases de configuração do ambiente Microsoft 365 para o projeto **LAB-A02**.

---

##  Fase 1: Gestão de Identidade e Licenciamento

### Atividades Realizadas:
* **Gestão de Identidade:** Criação do utilizador principal `trainee-LAB-A02`.
* **Licenciamento:** Atribuição da licença *Microsoft 365 Business Premium*.
* **Perfil:** Configuração do cargo como `Administrator` e departamento `IT`.
* **Segurança:** Criação do utilizador `support-LAB-A02` com bloqueio imediato de início de sessão.

---

##  Fase 06-15: Grupos e Microsoft Teams
### 1. Grupos de Segurança
* **Fixo:** Criado `GRP-IT-LAB-A02` com o membro `trainee-LAB-A02`.
* **Dinâmico:** Criado `GRP-DYN-IT-LAB-A02` com regra baseada no departamento "TI".

### 2. Colaboração de Projeto
* **Grupo M365:** Criado `M365-PROJECT-LAB-A02`.
* **Propriedade:** `trainee-LAB-A02` definido como Owner oficial.

### 3. Estrutura do Teams
* **Canais Públicos:** `Operations`, `Projects` e `Documentation`.
* **Canal Privado:** `Management` (Acesso restrito).

---

##  Fase 16-21: Exchange Online
Configuração de fluxos de comunicação e regras de transporte.

* **Shared Mailbox:** Criada `support-LAB-A02` com delegação de acesso total.
* **Distribuição:** Criada lista `DL-IT-LAB-A02` (`it-laba02@dominio.com`).
* **Mail Flow:** Implementação da regra `Disclaimer-LAB-A02` para anexar aviso de confidencialidade em e-mails internos.

---

##  Fase 22-30: SharePoint e Gestão Documental
### Site de Projeto (Ex 22-25)
* **Site:** `SITE-PROJECT-LAB-A02`.
* **Biblioteca:** `Docs-LAB-A02` com pastas `Policies`, `Projects` e `Reports`.
* **Segurança:** Interrupção de herança para dar acesso exclusivo ao `GRP-IT-LAB-A02`.

### SharePoint Avançado (Ex 26-30)
* **Biblioteca:** `Resources-LAB-A02`.
* **Segurança de Grão Fino:** Bloqueio da pasta `Templates` para garantir a integridade dos modelos.

---

##  Fase 31-40: Teams Sales e Identidade
* **Equipa Sales:** Criado grupo `M365-SALES-LAB-A02` com canais `Deals` e `Forecast`.
* **Identidade Mail:** Regra de transporte para prefixo `[INTERNAL]` em comunicações internas.
* **Suporte:** Reencaminhamento do alias de vendas para o técnico principal.

---

##  Fase 41-50: Gestão de RH e Validação Final
### Bloco 1: Recursos Humanos (Ex 41-45)
* **Segurança:** Grupo `GRP-HR-LAB-A02` para controlo de acessos.
* **Teams:** Equipa `TEAM-HR-LAB-A02` com canais `Recruitment` e `Training`.

### Bloco 2: Segurança e Auditoria (Ex 46-50)
* **Biblioteca RH:** `HRDocs-LAB-A02` com pastas `Contracts` e `EmployeeRecords`.
* **Permissões:** Atribuição do grupo de RH como membro oficial do site SharePoint.
* **Validação Global:** Verificação de todos os objetos via pesquisa portal com a tag `LAB-A02`.

---

> **Nota Final:** Todos os 50 exercícios foram documentados com prints numerados (01 a 36), garantindo a rastreabilidade de todas as configurações realizadas no Tenant.
