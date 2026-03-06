# Ansible - Deploy de WordPress com Infraestrutura como Código

Projeto desenvolvido durante os estudos do curso  
**"Ansible: implementando sua infraestrutura como código" da Alura.**

O objetivo do projeto é automatizar a configuração de servidores Linux utilizando **Ansible**, provisionando um ambiente completo com:

- Servidor Web (Apache)
- Banco de dados (MySQL)
- Aplicação WordPress

Toda a configuração da infraestrutura é feita utilizando **playbooks, roles, variáveis e templates**, seguindo o conceito de **Infraestrutura como Código (IaC)**.

---

# Tecnologias utilizadas

- Linux
- Ansible
- Apache
- MySQL
- WordPress
- SSH

---

# Estrutura do projeto

├── playbook.yml
├── hosts
├── group_vars
├── roles
├── templates
├── files

Descrição dos diretórios:

- **playbook.yml** → playbook principal responsável por orquestrar a instalação
- **hosts** → inventário com os servidores gerenciados
- **group_vars** → variáveis utilizadas nos playbooks
- **roles** → modularização das tarefas do Ansible
- **templates** → arquivos de configuração gerados dinamicamente
- **files** → arquivos utilizados durante a automação

---

# O que este projeto automatiza

- instalação de dependências
- configuração do servidor web
- configuração do banco de dados
- deploy do WordPress
- configuração das variáveis da aplicação

---

# Pré-requisitos

Para executar o projeto é necessário:

- Linux
- Ansible instalado
- acesso SSH aos servidores
- máquinas virtuais configuradas

---

# Execução do playbook

Edite o arquivo `hosts` com os endereços dos servidores e execute:


ansible-playbook -i hosts playbook.yml


---

# Aprendizados com este projeto

Durante o desenvolvimento deste projeto foram aplicados conceitos importantes de DevOps:

- automação de infraestrutura
- gerenciamento de configuração
- reutilização de tarefas com roles
- parametrização com variáveis
- uso de templates para configuração dinâmica

---

# Referência

Curso: Trilha DevOps
Ansible: implementando sua infraestrutura como código – Alura
