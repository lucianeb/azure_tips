# 💻 Guia Prático: Criação e Configuração de Máquina Virtual no Microsoft Azure

Este repositório contém **resumos**, **anotações** e **dicas práticas** sobre o uso da plataforma **Microsoft Azure**, com foco na criação e gerenciamento de **máquinas virtuais (VMs)**. Serve como material de apoio para estudos, testes e futuras implementações em ambientes de nuvem.

---

## ✨ Objetivos

- Praticar o processo completo de criação de uma VM no Azure.
- Documentar de forma clara os passos e decisões técnicas.
- Servir de base para estudos e reuso de boas práticas em projetos futuros.

---

## 📦 Pré-requisitos

- Conta na Microsoft (preferencialmente uma conta gratuita ou estudante com créditos).
- Cartão de crédito válido (para ativação da conta gratuita).
- Acesso ao portal [https://portal.azure.com](https://portal.azure.com).
- Git e GitHub configurados localmente.

---

## 🚀 Etapas para Criação de uma Máquina Virtual

### 1. Criar Conta no Azure

- Acesse [https://azure.microsoft.com/pt-br/free](https://azure.microsoft.com/pt-br/free)
- Escolha a opção **Conta Gratuita** ou **Estudante**.
- Complete o cadastro com e-mail, telefone e cartão de crédito.

### 2. Criar uma Máquina Virtual (VM)

- No Portal Azure, clique em **"Criar um recurso" > "Máquina Virtual"**.
- Preencha os campos:
  - **Grupo de Recursos**: criar novo ou usar existente.
  - **Nome da VM**: ex. `vm-azure-dev`.
  - **Região**: ex. `East US` (melhor compatibilidade com nível gratuito).
  - **Imagem**: `Ubuntu Server 20.04 LTS`.
  - **Tamanho**: `B1s` (incluso no nível gratuito).
  - **Autenticação**: escolher **senha** ou **chave SSH**.
  - **Portas abertas**: marque `SSH (22)`.

### 3. Acessar a VM via SSH

```bash
ssh azureuser@<ip-público>
