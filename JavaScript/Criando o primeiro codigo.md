  

## Explicação do código¹ :

````HTML
```html

<style></style> - <style> É conteudo e o codigo dentro delas é estilização da pagina.

<style>
body{background-color: rgb(0, 255, 255);}
</style>
///////////////////////////////////////

<script> </script> -São carregados após os codigos normalmente, porém pode ser feito após.
É um modo de interação para o codigo

 window.alert('Minha primeira mensagem kkk') - criará um alerta para a pagina com
a mensagem em 'mensagem'.

 window.confirm('O javaScript é suave ?') - criará uma mensagem de confirmação na tela com a
mensagem em 'mensagem'.FFFFDFGDFGDFGDF

	window.prompt('Qual o seu nome ?')  - Permite que o usuario escreva seu nome, porém para
ele ser mostrado nas tela é necessario uma variavel para guardar o valor.

	  <script>
        window.alert('Minha primeira mensagem kkk')
        window.confirm('O javaScript é suave ?')
  			window.prompt('Qual o seu nome ?')  
	</script>

````

  

  

# Código:

```JavaScript


<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
<style>
	body{background-color: rgb(0, 255, 255);}
</style>

</head>
<body>
	    <h1>Ola</h1>
    <p>Hoje eu to suave </p>

    <script>
        window.alert('Minha primeira mensagem kkk')
        window.confirm('O javaScript é suave ?')
				window.prompt('Qual o seu nome: ')
    </script>
    
</body>
</html>
```