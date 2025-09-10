# Procedure-View-Fun-o.

📚 Sistema de Biblioteca – Banco de Dados

Este projeto implementa um sistema de biblioteca com Procedures, Views e Funções em PostgreSQL.
O objetivo é praticar conceitos avançados de banco de dados, incluindo automação de processos, relatórios e regras de negócio.

🗂️Arquivo das Tabelas e Inserts
[Procedure Sistema de Biblioteca.pdf](https://github.com/user-attachments/files/22245249/Procedure.Sistema.de.Biblioteca.pdf)

🗂️ Estrutura do Banco de Dados
Tabelas principais

autor → Armazena os autores dos livros.

livro → Contém informações sobre os livros (título, ano, autor).

usuario → Representa os usuários da biblioteca.

emprestimo → Registra os empréstimos de livros pelos usuários.

⚙️ Funcionalidades
🔹 Procedures

cadastrar_usuario → Insere um novo usuário.

cadastrar_livro → Insere um novo livro.

registrar_devolucao → Atualiza a devolução de um empréstimo.

excluir_usuario → Remove um usuário e todos os seus empréstimos.

🔹 Views

livros_com_autores → Lista livros e seus autores.

usuarios_com_emprestimos → Usuários com livros emprestados.

emprestimos_em_aberto → Empréstimos sem data de devolução.

historico_emprestimos → Histórico completo (usuário, livro, autor, data).

qtd_emprestimos_por_usuario → Quantidade de empréstimos por usuário.

livros_mais_recentes → Livros publicados após 1950.

usuarios_com_mais_de_um_emprestimo → Usuários que pegaram mais de 1 livro.

🔹 Funções

autor_do_livro(p_id) → Retorna o autor de um livro.

livro_emprestado(p_id) → Verifica se o livro está emprestado ou disponível.

usuario_com_atraso(p_id) → Verifica se o usuário tem livros atrasados.

total_gasto_usuario(p_id) → Soma dos valores gastos em empréstimos.

📖 Conceitos

Procedures: blocos de código armazenados no banco que executam ações (INSERT, UPDATE, DELETE, lógica de negócio).

Views: consultas salvas que funcionam como "tabelas virtuais", simplificando relatórios e consultas.

Funções: retornam valores a partir de parâmetros, permitindo encapsular regras de negócio e cálculos.

🛠️ Tecnologias Utilizadas

PostgreSQL 15+

pgAdmin ou psql (para execução dos scripts)

👨‍💻 Autor

Projeto desenvolvido por Nicolas Alexandrino para a disciplina de Projeto de Banco de Dados – Sistema de Biblioteca.
