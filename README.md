# Assistencia_celulares

# 🔧 Sistema de Gerenciamento de Assistência Técnica

## 📌 Sobre o Projeto

Este projeto consiste no desenvolvimento de um sistema de gerenciamento para uma assistência técnica, com o objetivo de facilitar o controle de clientes, aparelhos e agendamentos de reparos.

O sistema permite organizar as informações, realizar cadastros, consultas, edições e exclusões, além de gerenciar os agendamentos de serviços de manutenção.

## 🎯 Objetivo

Desenvolver uma aplicação prática e intuitiva que auxilie no gerenciamento de uma assistência técnica, garantindo organização dos dados, segurança das informações e facilidade na administração dos serviços.

## ⚙️ Funcionalidades do Sistema

O sistema conta com as seguintes funcionalidades:

### 🔐 Autenticação e Segurança
- Login com usuário e senha.
- Armazenamento seguro de senhas utilizando hash bcrypt.
- Controle de sessão com expiração de 30 minutos.
- Redirecionamento para login quando a sessão expirar.
- Funcionalidade de logout.

### 👥 Gerenciamento de Clientes
- Cadastro de clientes com nome, CPF, telefone, e-mail e endereço.
- Validação de CPF com 11 dígitos.
- Proteção dos dados pessoais conforme a LGPD.
- Busca de clientes por nome, e-mail, telefone ou CPF.
- Edição dos dados cadastrados.
- Exclusão de clientes, desde que não possuam aparelhos vinculados.

### 📱 Gerenciamento de Aparelhos
- Cadastro de aparelhos com marca, modelo, IMEI, defeito relatado e cor.
- Associação de aparelhos aos clientes cadastrados.
- Validação de IMEI com 15 dígitos.
- Edição e exclusão de aparelhos.
- Bloqueio da exclusão quando existem agendamentos vinculados.

### 📅 Gerenciamento de Agendamentos
- Cadastro de agendamentos de reparos.
- Seleção do aparelho e serviço desejado.
- Definição de data e horário.
- Campo para observações.
- Status inicial definido como AGENDADO.
- Listagem de agendamentos organizada por data.
- Visualização das informações dos clientes e aparelhos relacionados.
- Reagendamento de serviços.
- Exclusão de agendamentos com confirmação.

## 📋 Requisitos Funcionais

| ID | Requisito |
|---|---|
| RF01 | Autenticação de usuário |
| RF02 | Sessão com tempo de expiração |
| RF03 | Tela principal |
| RF04 | Logout |
| RF05 | Cadastro de clientes |
| RF06 | Busca de clientes |
| RF07 | Edição de clientes |
| RF08 | Exclusão de clientes |
| RF09 | Cadastro de aparelhos com associação ao cliente |
| RF10 | Edição e exclusão de aparelhos |
| RF11 | Cadastro de agendamentos de reparo |
| RF12 | Listagem de agendamentos |
| RF13 | Reagendamento |
| RF14 | Exclusão de agendamentos |

## 🔒 Segurança e LGPD

O sistema considera boas práticas de segurança e proteção de dados pessoais, incluindo:

- Senhas armazenadas utilizando bcrypt.
- Controle de acesso por sessão.
- Expiração automática de sessões.
- Proteção das informações pessoais dos clientes.
- CPF armazenado de forma protegida