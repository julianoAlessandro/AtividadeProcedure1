# AtividadeProcedure1
Primeira lista ministrada pelo Professor de Banco de Dados Relacional Matheus
ALTER PROCEDURE aumentaSalario(@codigo int)
AS
BEGIN
 IF @codigo = 2
    SELECT salario_fixo * 1.2 AS AUMENTO_SALARIO,salario_fixo
    FROM dbo.vendedor
    WHERE faixa_comissao = 'B'
IF @codigo = 3
    SELECT salario_fixo * 1.3 AS AUMENTO_SALARIO,salario_fixo
    FROM dbo.vendedor
    WHERE faixa_comissao = 'B'
IF @codigo = 4
    SELECT salario_fixo * 1.4 AS AUMENTO_SALARIO,salario_fixo
    FROM dbo.vendedor
    WHERE faixa_comissao = 'B'
END;
