# atividade5_091023

<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <script>

        function NomedeLista()
        {

            var nomeTodo, UltimoNome, UltimoEspaco, ultimaLetra, primeiroNome;
            
            nomeTodo = (document.Nome.nome_completo.value);
            UltimoEspaco = (nomeTodo.lastIndexOf(" "));
            UltimoNome = (nomeTodo.substring(UltimoEspaco));
            primeiroNome = (nomeTodo.substr(0,UltimoEspaco));

            document.writeln("<p> Entrada : " + nomeTodo + ".</p>");
            document.writeln("<p> Saída : " + UltimoNome + ", " + primeiroNome + ".</p>");

        }

    </script>
    <Form name="Nome">

        Informe aqui o nome a ser armazenado: <input type="text" name="nome_completo" placeholder="Ex: Nome Sobrenome...">
        <input type="submit" name="Entrada" value="Enviar" onclick="NomedeLista()">
    
    </Form>
</body>
</html>
