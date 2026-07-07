# Registro de Decisões

Este documento registra as principais decisões técnicas tomadas durante o desenvolvimento do projeto, bem como a justificativa de cada uma delas.

---

## ADR-001 — Utilizar Git para versionamento

**Data:** 05/07/2026

### Decisão

O projeto será versionado utilizando Git e hospedado no GitHub.

### Justificativa

Manter o histórico das alterações, facilitar a evolução do projeto e demonstrar boas práticas de desenvolvimento.

---

## ADR-002 — Não versionar os dados brutos

**Data:** 05/07/2026

### Decisão

Os arquivos CSV do dataset serão ignorados pelo Git através do `.gitignore`.

### Justificativa

Os dados brutos possuem grande volume e podem ser obtidos diretamente no Kaggle. O repositório deve conter apenas código, documentação e demais arquivos necessários para reproduzir o projeto.

---

## ADR-003 — Documentar o projeto desde o início

**Data:** 05/07/2026

### Decisão

A documentação será construída ao longo do projeto, acompanhando sua evolução.

### Justificativa

Manter o contexto das decisões, facilitar a manutenção e tornar o projeto mais compreensível para outros profissionais.