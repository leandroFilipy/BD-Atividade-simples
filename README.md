🏥 Modelagem de Banco de Dados – Sistema de Consultas Médicas
📌 Descrição
Este repositório contém uma planilha desenvolvida no início da unidade curricular de Banco de Dados, com o objetivo de praticar a criação de tabelas relacionadas simulando um sistema de consultas médicas.

As tabelas representam os principais elementos envolvidos no acompanhamento médico de gestantes e recém-nascidos, com foco em organização de dados, uso de chaves primárias e estrangeiras, e simulação de relacionamentos reais.

🧱 Estrutura das Tabelas
👩‍⚕️ Médico
Contém informações dos profissionais responsáveis pelos atendimentos.

Atributos:

id_medico (PK)

nome

especialidade

crm

🤰 Mãe
Registra dados das pacientes gestantes atendidas na unidade.

Atributos:

id_mae (PK)

nome

cpf

data_nascimento

👶 Bebê
Tabela associada à mãe, registrando informações do recém-nascido.

Atributos:

id_bebe (PK)

nome

data_nascimento

peso

id_mae (FK)

📆 Consulta
Representa as consultas médicas realizadas, vinculando mãe e médico.

Atributos:

id_consulta (PK)

data

horario

id_mae (FK)

id_medico (FK)

🔗 Relacionamentos
Uma mãe pode ter um ou mais bebês

Um médico pode realizar várias consultas

Uma consulta sempre envolve uma mãe e um médico

Um bebê está sempre vinculado a uma mãe

Essas relações simulam um banco relacional real, com integridade entre as entidades e foco na rastreabilidade de dados.

🎯 Objetivos da atividade
Praticar os conceitos fundamentais de modelagem relacional

Representar entidades reais com atributos e relacionamentos

Trabalhar com a ideia de chaves primárias e chaves estrangeiras

Estimular o pensamento lógico e estruturado no design de bancos de dados
