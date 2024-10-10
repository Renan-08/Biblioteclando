### Escopo do Projeto

*Título do Projeto*: Sistema de gerenciamento multimeios 

*Objetivo*: Desenvolver um aplicativo de fácil utilização para gerenciar o acervo, empréstimos e devoluções de livros, permitindo que alunos possam consultar o catálogo online e realizar reservas de exemplares.

#### Funcionalidades Principais:
1. *Cadastro de Livros*:
   - Registro de novos livros no sistema, com dados como título, autor, ISBN, gênero, etc.
   - Atualização de dados dos livros existentes no sistema.

2. *Empréstimo e Devolução*:
   - Gerenciamento de empréstimos de livros, associando-os a um aluno
   - Controle de datas de devolução e renovação automática ou manual.

3. *Consulta e Reserva de Livros*:
   - Busca de livros no catálogo por título, autor, ISBN ou gênero.
   - Reservas de livros disponíveis ou em fila de espera para exemplares emprestados.

4. *Usuários*:
   - Cadastro e autenticação de alunos, professores e bibliotecários.
   - Controle de permissões para cada tipo de usuário.

5. *Relatórios*:
   - Emissão de relatórios sobre livros mais emprestados, atrasos na devolução, etc.

6. *Notificações*:
   - Notificações por e-mail ou push para lembrar sobre a data de devolução dos livros.

7. *Integração com Sistema de Biblioteca Física*:
   - Sincronização entre o sistema do aplicativo e a biblioteca física.

#### Tecnologias:
- *Front-end*: Javascript e PHP 
- *Back-end*: Python 
- *Banco de Dados*: MySQL para armazenar os dados da biblioteca.
- *Autenticação*: JWT em análise para uso

#### Cronograma:
1. *Planejamento (2 mês)*:
   - Definir requisitos e desenhar as telas do aplicativo.
2. *Desenvolvimento (3 meses)*:
   - Implementação do front-end e back-end.
3. *Testes e Ajustes (1 mês)*:
   - Testes com usuários finais e correções de bugs.
4. *Entrega (Versão Demo) e Treinamento (2 semanas)*:
   - Treinamento para bibliotecários e lançamento oficial
  
### Árvore de Problema

*Problema Central*: Dificuldade de gerenciamento eficiente do multimeios e do controle de empréstimos na biblioteca da escola.

*Causas*:
1. *Gestão manual de acervo*:
   - Controle de livros feito em cadernos ou planilhas.
   - Erros na catalogação e dificuldade para localizar livros seja por empréstimo ou não.

2. *Controle de empréstimos desatualizado*:
   - Dificuldade no sistema físico utilizado para registrar e acompanhar os empréstimos.
   - Alunos e professores não têm visibilidade sobre o status dos livros.

3. *Falta de acesso remoto ao catálogo*:
   - Os usuários precisam ir fisicamente à biblioteca para consultar ou remotamente.

*Consequências*:
1. *Atrasos na devolução de livros*: 
   - Falta de lembretes automáticos sobre prazos de devolução.

2. *Desorganização e extravio de livros*:
   - Perda ou dificuldade de encontrar exemplares.

3. *Ineficiência no atendimento ao usuário*:
   - Mais tempo gasto para realizar buscas e empréstimos.

### Código da tabela multimeios 
```
create database multimeios
default character set utf8mb4
default collate utf8mb4_general_ci;




create table livros(
reg  int not null auto_increment,
cdd varchar (30),
acervo date,
autor varchar (150),
titulo varchar (150) not null,
volume tinyint,
exemplar int,
primary key (reg)
) default character set = utf8mb4;
```
