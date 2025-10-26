# DriveJoy-RLA

9. Luis, Wanessa e Nicolas: Sistema de Locadora de Veículos (DriveJoy)
Objetivo: Gerenciar a frota de veículos, clientes e o processo de aluguel e devolução.

•	Dados (Frota):
o	placas: Array de strings (chave única).
o	modelos: Array de strings.
o	valorDiaria: Array de números.
o	estaAlugado: Array de booleanos.

•	Dados (Clientes):
o	nomesCliente: Array de strings.
o	cnhCliente: Array de strings (chave única).


•	Funções (Menu):

1.	Cadastrar Cliente: Pede nome e CNH.

2.	Cadastrar Veículo: Pede placa, modelo e valor da diária. Inicializa estaAlugado como false e alugadoParaCNH como "".

3.	Alugar Veículo:
	Lista os veículos disponíveis (estaAlugado == false).
	Pede a placa do carro desejado (acha indexCarro).
	Pede a CNH do cliente (acha indexCliente).
	Muda estaAlugado[indexCarro] para true.
	Salva cnhCliente[indexCliente] em alugadoParaCNH[indexCarro].

4.	Devolver Veículo:
	Pede a placa do carro (acha indexCarro).
	Verifica se estaAlugado[indexCarro] é true.
	Muda estaAlugado[indexCarro] para false.
	Limpa alugadoParaCNH[indexCarro] (coloca "").
	(Opcional difícil): Pergunta quantos dias ficou e calcula o total a pagar.

5.	Listar Frota Completa: Mostra todos os carros, e se está alugado, mostra para quem (usando a CNH).

6.	Sair.
