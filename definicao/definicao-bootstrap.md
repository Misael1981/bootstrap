# Bootstrap: O que é, Documentação, como e quando usar

Quando vamos criar um site, precisamos tomar diversas decisões, como qual banco de dados, linguagem e framework vamos usar, ou ainda onde faremos o deploy da aplicação.

Porém, um ponto muito importante é conseguir deixar nossa página com um visual bacana, customizando cores, fontes, margens e assim por diante. Para isso, precisamos estilizá-la por meio de inúmeras classes do CSS, o que não é uma tarefa simples para todos que desenvolvem.

Pensando nisso, vamos ver uma forma de estruturar e estilizar suas aplicações com Bootstrap.

## Bootstrap: O que é?

**Bootstrap** é um framework front-end que fornece estruturas de CSS para a criação de sites e aplicações responsivas de forma rápida e simples. Além disso, pode lidar com sites de desktop e páginas de dispositivos móveis da mesma forma.

Originalmente, o Bootstrap foi desenvolvido para o Twitter por um grupo de desenvolvedores liderados por Mark Otto e Jacob Thornton Logo e se tornou uma das estruturas de front-end e projetos de código aberto mais populares do mundo.

Antes de ser uma estrutura de código-fonte aberto, o Bootstrap era conhecido como Twitter Blueprint. Após alguns meses de desenvolvimento, o Twitter realizou sua primeira Hack Week: o projeto ganhou uma grande popularidade quando desenvolvedores de todos os níveis de habilidade usaram o framework sem qualquer orientação externa. Após o evento, ele serviu como guia de estilo para o desenvolvimento de ferramentas internas na empresa por mais de um ano antes de seu lançamento se tornar público.

## Como o Bootstrap é distribuído?

Geralmente, o Bootstrap é distribuído usando o [site oficial](https://getbootstrap.com/) e [npm](https://www.npmjs.com/). Você também pode criar sua própria distribuição usando o código-fonte, ou por meio da própria rede de distribuição de conteúdo conhecida como CDN do Bootstrap. Um CDN permite que um site da web recupere com frequência arquivos públicos usados ​​de servidores distribuídos globalmente.

## Como instalar o Bootstrap?

Na página de download oficial você encontra com detalhes todas as formas de instalar o Bootstrap.

Nós vamos aprender a instalá-lo via CDN.

Para alcançar o mesmo resultado deste artigo na sua instalação, crie uma pasta e um arquivo chamado index.html.

No arquivo, inclua o seguinte código:

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Exemplo Bootstrap</title>
</head>
<body>
    <h1>O Bootstrap é bem legal</h1>
</body>
</html>
```

Nosso resultado será:

Confira o código completo:

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-EVSTQN3/azprG1Anm3QDgpJLIm9Nao0Yz1ztcQTwFspd3yD65VohhpuuCOmLASjC" crossorigin="anonymous">
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/js/bootstrap.bundle.min.js" integrity="sha384-MrcW6ZMFYlzcLA8Nl+NtUVF0sA7MsXsP1UyJoMp4YLEuNSfAP+JcXn/tWtIaxVXM" crossorigin="anonymous"></script>
    <title>Exemplo Bootstrap</title>
</head>
<body>
    <h1>O Bootstrap é bem legal</h1>
</body>
</html>
```

## Componentes do Bootstrap

Na documentação, você encontra uma série de componentes como referência para suas próprias criações, como alertas, botões, menu, formulários, entre muitos outros.

### [Voltar ao README](../README.md)