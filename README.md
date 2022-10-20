# Banco-de-Dados-T.
<!-- Formulario de Dados -->
<!DOCTYPE html>
<html>
<head>
	<meta charset="utf-8">
	<meta name="viewport" content="width=device-width, initial-scale=1">
	<title>Formulario</title>
</head>
<body>
	<form action="/pagina-processa-dados-do-form" method="post">
		<fieldset>
			<legend>Dados Gerais</legend>

			<label for="nome">Nome:</label>
			<input type="text" minlength="3" id="nome"  required />

			<label for="data_nascimento">Data de Nascimento:</label>
			<input type="text" id="data_nascimento" required />

			<label for="cpf">CPF:</label>
			<input type="text" minlength="11" maxlength="11" id="cpf" required />

			<label for="tel">Tel. Celular</label>
			<input type="tel" max="13" name="tel" placeholder="83-99999-9999" pattern="[0-9]{2}-[0-9]{5}-[0-9]{4}" required />
		</fieldset>	

		<fieldset>
			<legend>Endereço</legend>

			<label for="tipo_endereco">Tipo:</label>
			<select id="tipo_endereco">
				<option value="">Selecione</option>
				<option value="rua">Rua</option>
				<option value="estrada">Estrada</option>
				<option value="rodovia">Rodovia</option>
				<option value="outro">Outro</option>
			</select>

			<label for="logradouro_endereco">Logradouro:</label>
			<input type="text" id="logradouro_endereco" />

			<label for="numero_endereco">N°:</label>
			<input type="text" id="numero_endereco"/>

			<label for="complemento_endereco">Complemento:</label>
			<input type="text" id="complemento_endereco">
		</fieldset>	

		<fieldset>
			<legend>Fale Conosco</legend>

			<label for="tipo_msg">Tipo de Mensagem:</label>
			<input type="radio" name="tipo_msg" value="Sugestão"/>
			<input type="radio" name="tipo_msg" value="Crítica"/>
			<input type="radio" name="tipo_msg" value="Elogio"/>

		 	<label for="msg">Mensagem:</label>
		 	<textarea id="msg"></textarea>
		</fieldset>

		<fieldset>
			<button type="submit">Enviar sua mensagem</button>
			<button type="reset">Limpar o Formulário</button>
		</fieldset>
	</form>
</body>
</html>
