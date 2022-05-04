# Avaliando o aprendizado.

## Módulo 1
1. Assinale a alternativa que corresponde à afirmativa que define o que é entendido por escopo de variáveis na linguagem Javascript.
> A) Ao falarmos de escopo de variáveis, nós nos referimos ao local de nosso código onde determinada variável pode ser acessada.
2. Considerando o fragmento de código a seguir, assinale a alternativa correspondente à sua saída – o que será exibido no comando “console.log”, na última linha.
```js
var texto = "Texto atribuído à variável";
imprimirTexto();
function imprimirTexto(){
var texto = "Novo texto atribuído à variável";
}
console.log(texto);
```
> B) "Texto atribuído à variável".
---
## Módulo 2
1. Assinale a alternativa que corresponde ao código que, fazendo uso do Framework jQuery, permite adicionar uma tag <h1>, contendo o texto “Título inicial”, como primeiro elemento dentro da tag <body>, considerando o fragmento de código HTML abaixo.
```html
<!doctype html>
<html lang="pt-BR"><head>
<meta charset="utf-8">
<title>Página HTML</title>
<script type="text/javascript" src="https://code.jquery.com/jquery-3.5.1.js"></script>
</head>
<body>
<div id="lipsum">
<p> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed justo ipsum, rhoncus at orci vel, aliquam consequat lorem. Integer congue enim quis semper mattis. Aenean augue libero, maximus et odio nec, malesuada tristique felis. Donec dignissim libero id pulvinar faucibus. Phasellus blandit justo quam. Integer ex massa, rhoncus eu libero quis, fermentum feugiat odio. Sed tellus purus, fermentum ac euismod et, mattis at nunc. Nunc nisl leo, dapibus eget lorem id, congue lobortis ipsum. </p>
</div>
</body>
</html>

```
> D) $( 'body' ).before(‘<h1>Título inicial</h1>’).</p>
2. Através do Framework jQuery, é possível manipular os elementos da árvore DOM e o seu conteúdo. Nesse contexto, assinale a afirmativa que demonstra como remover o conteúdo de todas as tags <p> de uma página HTML.
> C) $(‘p’).html(‘’).
---
## Módulo 3
1. Em algumas situações, pode ser necessário manipular os elementos ou o conteúdo da página antes que eles sejam apresentados ao usuário. Nesse sentido, assinale a alternativa que corresponda ao evento que deve ser utilizado para manipulação da página HTML antes que seu conteúdo (imagens, textos etc.) seja totalmente carregado.
> D) $(document).ready().
2. A partir do código a seguir, é desejado que, ao ser clicado, o link “Exibir alerta” apenas exiba na tela uma caixa de diálogo (alert), sem, entretanto, levar o usuário à página indicada em seu atributo href (pagina.html). Assinale a alternativa correspondente aos códigos que preenchem as lacunas e que deverão ser utilizados para realizar essa tarefa.
```html
<!doctype html>
<html lang="pt-BR"><head>
<meta charset="utf-8">
<title>Página HTML</title>
<script type="text/javascript" src="https://code.jquery.com/jquery-3.5.1.js"></script>
</head>
<body>
<div id="lipsum">
<p> Lorem ipsum dolor sit amet, consectetur adipiscing elit. </p>
</div>
<script type="text/javascript">
$(function() {
$( '#lipsum' ).append("<a id='link_alerta' href='pagina.html'>Exibir alerta</a>");
$('#_ _ _ _ _')._ _ _ _ _(' _ _ _ _ _ ', function(event){
_ _ _ _.preventDefault();
alert('O novo link foi clicado');
});
});
</script>
</body>
</html>
```
> B) link_alerta/ on/ click/ event.
---
## Módulo 4
1. Em relação ao método jQuery $.ajax, utilizado para a realização de requisições AJAX, assinale a alternativa correta relativa à sua sintaxe e às suas propriedades.
> Além de acessar recursos externos de forma assíncrona, esse método permite a manipulação dos dados obtidos, possibilitando que eles sejam, por exemplo, acrescentados aos demais conteúdos já existentes na página.
2. Considere o fragmento de código abaixo, onde temos uma string JSON como retorno de uma requisição AJAX, e o método .done(), que recebe como parâmetro tal string, representada pela variável result.

A partir desse código, assinale a alternativa correta que corresponda às lacunas do código quanto à forma de acessar o nome do aluno, a sua nota e a disciplina “Matematica”.
```js
//os dados abaixo estão contidos na variável result, visível na função .done
{
"id": 1,
"nome": "Aluno",
"nota": 10,
"disciplinas": ["Matematica", "Geografia"]
}
...
.done(function(result){
var nomeAluno = _ _ _ _ _ ;
var notaAluno = _ _ _ _ _ ;
var disciplina = _ _ _ _ _ ;
})
...
```
> B) result.nome/ result.nota/ result.disciplinas[0].
