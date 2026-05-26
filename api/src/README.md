 🎓 Aluno Online

O **Aluno Online** é uma API REST desenvolvida em Java para o gerenciamento de uma instituição de ensino. O sistema permite o controle completo de alunos, professores, disciplinas e o processo de matrícula, garantindo a persistência dos dados em um banco de dados relacional.

## 📝 Explicação do Projeto
O objetivo principal deste projeto é fornecer uma infraestrutura de backend para gerenciar os fluxos operacionais de uma escola ou universidade. Com ele, é possível cadastrar e gerenciar o corpo docente e discente, organizar as disciplinas ofertadas e realizar a vinculação de alunos a essas disciplinas por meio do módulo de matrícula.

---

## 🏛️ Descrição da Arquitetura Utilizada
O projeto foi desenvolvido seguindo o padrão de arquitetura **CRUD (Create, Read, Update, Delete)** em camadas, separando as responsabilidades do sistema da seguinte forma:

- **Controller (Camada de Rest/Endpoints):** Responsável por expor os endpoints da API, receber as requisições HTTP (GET, POST, PUT, DELETE) e retornar as respostas adequadas.
- **Service (Camada de Negócio):** Onde ficam as regras de negócio do sistema e as validações necessárias antes de persistir ou alterar os dados.
- **Repository / DAO (Camada de Persistência):** Camada responsável pela comunicação direta com o banco de dados PostgreSQL, executando as operações SQL.
- **Model / Entity (Camada de Domínio):** Classes que representam as tabelas do banco de dados (Aluno, Professor, Disciplina, MatriculaAluno).

---

## 💻 Detalhamento do Código e Tecnologias

### Tecnologias Utilizadas:
- **Linguagem:** Java
- **Banco de Dados:** PostgreSQL
- **Ferramenta de Testes de API:** Insomnia
- **Gerenciador de Banco de Dados:** DBeaver

### Funcionalidades Implementadas:
- **CRUD Aluno:** Cadastro, listagem, consulta por ID, atualização e remoção de alunos.
- **CRUD Professor:** Cadastro, listagem, consulta por ID, atualização e remoção de professores.
- **CRUD Disciplina:** Cadastro, listagem, consulta por ID, atualização e remoção de disciplinas.
- **Matrícula de Alunos:** Implementação de todos os métodos de negócio para a classe `MatriculaAluno` conforme trabalhado em sala de aula.

---

## 🚀 Testes das Requisições (Insomnia)

Abaixo estão os registros das validações das rotas da API realizando as operações de criação, leitura, atualização e deleção.

### 🔹 CRUD Aluno

<img width="1919" height="1079" alt="Captura de tela 2026-05-26 183202" src="https://github.com/user-attachments/assets/7a6d0500-ad30-400a-bd03-745fce247dc7" />
<img width="1919" height="1079" alt="Captura de tela 2026-05-26 184342" src="https://github.com/user-attachments/assets/e40cf514-8aee-45db-b32e-7ab6673b77e3" />
<img width="1915" height="1077" alt="Captura de tela 2026-05-26 184322" src="https://github.com/user-attachments/assets/630468ef-0b41-4b40-8a09-113e81888e46" />
<img width="1919" height="1079" alt="Captura de tela 2026-05-26 184259" src="https://github.com/user-attachments/assets/c700b2ee-38c6-46ae-9b2c-c1300a7f20e4" />
<img width="1917" height="1079" alt="Captura de tela 2026-05-26 184236" src="https://github.com/user-attachments/assets/b331a190-6a98-4b67-98d7-fdb78d4cbaf9" />


### 🔹 CRUD Professor
<img width="1914" height="1079" alt="Captura de tela 2026-05-26 185356" src="https://github.com/user-attachments/assets/75725b83-f1fc-48e3-a160-e0b5d4f5b638" />
<img width="1911" height="1079" alt="Captura de tela 2026-05-26 185343" src="https://github.com/user-attachments/assets/8e71c51c-3fc1-4ecf-a3e7-ce2a9dfeb6fc" />
<img width="1917" height="1079" alt="Captura de tela 2026-05-26 185535" src="https://github.com/user-attachments/assets/8e3139f4-523b-4896-83d9-10cfdc9ac2dc" />
<img width="1908" height="1079" alt="Captura de tela 2026-05-26 185523" src="https://github.com/user-attachments/assets/129fc017-005d-4ad0-b1af-a12a786988b4" />
<img width="1918" height="1079" alt="Captura de tela 2026-05-26 185411" src="https://github.com/user-attachments/assets/4e5e288e-8b18-409b-bbda-132d1fd5965d" />


### 🔹 CRUD Disciplina & Matrícula
<img width="1919" height="1079" alt="Captura de tela 2026-05-26 185944" src="https://github.com/user-attachments/assets/03414541-3f2d-4c2f-8765-919e89d91958" />
<img width="1919" height="1079" alt="Captura de tela 2026-05-26 185929" src="https://github.com/user-attachments/assets/588a48a1-7d3e-470b-a0ea-f0161fb98748" />
<img width="1919" height="1079" alt="Captura de tela 2026-05-26 185835" src="https://github.com/user-attachments/assets/bcf4f966-82b3-499d-8c0f-24786a4de3b2" />
<img width="1919" height="1079" alt="Captura de tela 2026-05-26 185815" src="https://github.com/user-attachments/assets/855f089a-87e5-4d44-aa21-4f3618471ffb" />
<img width="1919" height="1079" alt="Captura de tela 2026-05-26 185747" src="https://github.com/user-attachments/assets/eed643b5-7a7f-4b2a-a914-e207016a3405" />
<img width="1919" height="1079" alt="Captura de tela 2026-05-26 185734" src="https://github.com/user-attachments/assets/3bc3e2a6-64f6-4b1e-a2c3-4dcfc2e6e5d0" />
<img width="1919" height="1079" alt="Captura de tela 2026-05-26 185705" src="https://github.com/user-attachments/assets/0e7095db-5462-40aa-a188-bf691079a68f" />


---

## 🗄️ Banco de Dados (DBeaver)

Visualização das tabelas no PostgreSQL através do DBeaver, contendo os dados que foram devidamente populados durante a fase de testes.

### 📊 Tabela: Aluno
<img width="1919" height="1079" alt="Captura de tela 2026-05-26 190028" src="https://github.com/user-attachments/assets/6e370c19-8e4d-4f62-8d10-a341618ebd1c" />
<img width="1919" height="1079" alt="Captura de tela 2026-05-26 184458" src="https://github.com/user-attachments/assets/8a4be78f-2577-48e6-9c0b-3ad45acac87a" />




### 📊 Tabela: Professor
<img width="1919" height="1079" alt="Captura de tela 2026-05-26 190158" src="https://github.com/user-attachments/assets/c8136cff-57ff-4f27-b64c-ae9f9ce4bb7b" />
<img width="1919" height="1079" alt="Captura de tela 2026-05-26 184510" src="https://github.com/user-attachments/assets/504245be-b702-41d0-88b1-cddf93a16ba4" />


 
 
 
 
