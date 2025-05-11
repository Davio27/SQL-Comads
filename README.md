
#🔍 SELECT
Usado para consultar e recuperar dados de uma tabela.
Exemplo:

SELECT * FROM clientes;
(Seleciona todas as colunas da tabela clientes.)




#➕ INSERT INTO
Usado para inserir novos registros em uma tabela.
Exemplo:

INSERT INTO clientes (nome, idade) VALUES ('João', 30);
(Insere um cliente chamado João com 30 anos.)



#✏️ UPDATE
Usado para atualizar dados existentes em uma tabela.
Exemplo:

UPDATE clientes SET idade = 31 WHERE nome = 'João';
(Atualiza a idade de João para 31.)



#❌ DELETE
Usado para excluir registros de uma tabela.
Exemplo:

DELETE FROM clientes WHERE nome = 'João';
(Remove o cliente chamado João.)



#🛠️ CREATE TABLE
Usado para criar uma nova tabela no banco de dados.
Exemplo:

CREATE TABLE clientes (
  id INT,
  nome VARCHAR(100),
  idade INT
);
(Cria a tabela clientes com colunas id, nome e idade.)



#🧱 ALTER TABLE
Usado para modificar a estrutura de uma tabela existente.
Exemplo:

ALTER TABLE clientes ADD email VARCHAR(100);
(Adiciona a coluna email na tabela clientes.)



#💣 DROP TABLE
Usado para excluir uma tabela permanentemente.
Exemplo:

DROP TABLE clientes;



#⚡ CREATE INDEX
Usado para criar um índice e melhorar a performance de consultas.
Exemplo:

CREATE INDEX idx_nome ON clientes (nome);
(Cria um índice chamado idx_nome na coluna nome.)



#🗑️ DROP INDEX
Usado para remover um índice existente.
Exemplo:

DROP INDEX idx_nome;



#🔗 JOIN
Usado para combinar dados de duas ou mais tabelas com base em uma relação.
Exemplo:

SELECT pedidos.id, clientes.nome
FROM pedidos
INNER JOIN clientes ON pedidos.cliente_id = clientes.id;
(Combina pedidos com nomes de clientes.)



#📊 ORDER BY
Usado para ordenar os resultados de uma consulta.
Exemplo:

SELECT * FROM clientes ORDER BY idade DESC;
(Ordena os clientes da maior para a menor idade.)



#🔢 COUNT()
Usado para contar o número de registros.
Exemplo:

SELECT COUNT(*) FROM clientes;
(Retorna o número total de clientes.)



#📦 GROUP BY
Usado para agrupar registros com valores iguais em uma ou mais colunas.
Exemplo:

SELECT idade, COUNT(*) FROM clientes GROUP BY idade;
(Conta quantos clientes há em cada faixa etária.)



#🚫 HAVING
Usado para filtrar grupos após o GROUP BY.
Exemplo:

SELECT idade, COUNT(*) 
FROM clientes 
GROUP BY idade 
HAVING COUNT(*) > 1;
(Mostra faixas etárias com mais de 1 cliente.)



#🔍 LIKE
Usado para buscar padrões em uma coluna.
Exemplo:

SELECT * FROM clientes WHERE nome LIKE 'Jo%';
(Seleciona nomes que começam com "Jo".)



#✅ IN
Usado para filtrar registros que estejam dentro de uma lista de valores.
Exemplo:

SELECT * FROM clientes WHERE idade IN (25, 30, 35);



#❎ NOT IN
Usado para excluir registros com valores indesejados.
Exemplo:

SELECT * FROM clientes WHERE idade NOT IN (18, 21);



#📏 BETWEEN
Usado para selecionar valores dentro de um intervalo.
Exemplo:

SELECT * FROM clientes WHERE idade BETWEEN 20 AND 30;



#🕳️ IS NULL
Usado para verificar se um valor é nulo (sem valor).
Exemplo:

SELECT * FROM clientes WHERE email IS NULL;
![image](https://github.com/user-attachments/assets/29187879-2633-4643-894f-f47ef5e51ab1)

