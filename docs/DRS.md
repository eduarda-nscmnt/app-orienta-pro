# Documento de Requisitos de Software (DRS)

## 1. Introdução

O documento apresenta os requisitos de orientação profissional voltado para os estudantes de ensino médio.

### 1.1 Visao Geral

O sistema tem como objetivo auxiliar na escolha da carreira, oferecendo testes vocacionais e informações sobre profissões, cursos e mercado de trabalho.

### 1.2 Objetivos do Sistema

.Ajudar estudantes a escolherem uma profissão; Fornecer testes vocacionais; Apresentar informações sobre o curso e área; Mostrar média salarial e mercado de trabalho.

### 1.3 Público Alvo

.Estudantes do ensino médio; Jovens indecisos. 
---

## 2. Escopo do Sistema

### 2.1 Escopo Incluído

.Cadastro e Login de usuários;Testes vocacionais;Visualização de profissões;Informações sobre cursos e mercado. 

### 2.1 Escopo Incluído

.Consultoria com profissionais;Emissão de certificados. 

---

## 3. Requisitos Funcionaís

### RF00 - Cadastro de usuário (O sistema deve pedir nome, e-mail e senha)

### RF01 - Login (O sistema deve pedir e-mail e senha)

### RF02 - Teste vocacional (O sistema deve disponibilizar perguntas sobre interesses e habilidades)

### RF03 - Resultado do teste (O sistema deve sugerir profissões com base nas respostas)

### RF04 - Listagem de profissões (O sistema deve exibir descrição, salário médio e área)

### RF05 - Busca ( O usuário deve pesquisar por nome ou área)

---

## 4. Requisitos Não Funcionais

### RNF00 - Usabilidade (Interface simples e fácil de usar)

### RNF01 - Desempenho (Resposta em até 5 segundos)

### RNF02 - Segurança (Proteção dos dados do usuário)

### RNF03 - Compatibilidade (Funcionamento em Android)

## 5. Arquitetura Técnica 

### 5.1 Stacks

#### 5.1.1 Stack Backend 

.JavaScript;Node.js;MySQL 
.Framework: Django

#### 5.1.2 Stack Frontend

.HTML, Css e JavaScript 

#### 5.1.7 Banco de Dados

.MySQL (Sistema de gerenciamento de banco de dados relacional responsável por armazenar informações dos usuários e testes vocacionais);
Tabelas para usuários,testes,resultados e profissões; Relacionamento entre dados para garantir integridade das informações.

## 6. Modelo de Dados

.O sistema será composto pelas seguintes entidades:

Usuário
.Id_usuario (chave primária); Nome, Email; Senha.

Teste Vocacional
.Id_teste (chave primária); Id_usuario (chave estrangeira); Respostas; Resultado.

Profissão
.Id_profissao (chave primária; Nome; Escrição; Área; Salario_medio.

Curso
.Id_curso (chave primária); Nome; Descrição; Duração; Área.

Relacionamentos
.Um usuário pode realizar vários testes;Um teste gera sugestões de profissões;Uma profissão pode estar ligada a um ou mais cursos.
