# 🚀 Flash Sales API - Infraestrutura DevOps

Este repositório contém a infraestrutura de automação, implantação e operação da **Flash Sales API**, desenvolvida com base nas melhores práticas de Engenharia DevOps.

---

## 🛠️ Tecnologias e Ferramentas Utilizadas

- **Aplicação:** Node.js, TypeScript, Jest
- **Containerização:** Docker (Multi-stage build)
- **Orquestração:** Docker Compose
- **Integração e Entrega Contínua (CI/CD):** GitHub Actions
- **Controlo de Versão:** Git & GitHub

---

## 🏗️ Justificativa da Arquitetura DevOps

A arquitetura foi projetada com foco nos três pilares fundamentais do DevOps: **Escalabilidade, Segurança e Confiabilidade**.

1. **Imutabilidade e Containerização (Dockerfile Multi-Stage):**
   - A adoção de *Multi-stage builds* garante imagens leves, contendo apenas as dependências necessárias para a execução em produção, reduzindo a superfície de ataque e otimizando o consumo de recursos.

2. **Automação de CI/CD (GitHub Actions):**
   - Cada alteração enviada para o repositório dispara um pipeline automatizado que instala dependências, compila o código TypeScript, executa os testes unitários/integrados via Jest e valida o build do container. Isso evita regressões de código e garante alta confiabilidade nas entregas.

3. **Reprodutibilidade do Ambiente (Docker Compose):**
   - O uso de infraestrutura declarativa assegura que qualquer desenvolvedor ou engenheiro de operações possa subir exatamente o mesmo ambiente de execução de forma padronizada.

---

## 📋 Como Executar o Projeto Localmente (Sem Docker)

Como o projeto utiliza Node.js e TypeScript, podes executá-lo diretamente com os seguintes passos:

### Pré-requisitos
- Node.js (versão 18 ou superior)
- NPM instalado

### Passo a Passo

1. Instalar as dependências do projeto:
   ```bash
   npm install