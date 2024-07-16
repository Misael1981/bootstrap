# Semântica no HTML

O Bootstrap 5 é um dos frameworks de front-end mais populares e amplamente utilizados para o desenvolvimento de interfaces web responsivas. Ele oferece uma ampla gama de componentes prontos para uso, como modals (modais) e cards (cartões), que ajudam os desenvolvedores a criar rapidamente layouts atraentes. No entanto, esses componentes geralmente vêm com uma quantidade excessiva de tags genéricas, como divs, que podem prejudicar a semântica do código HTML. Vamos entender a importância de refatorar essas tags genéricas em componentes do Bootstrap 5 e como isso contribui para um código HTML mais semântico?

## - Semântica no HTML:

A semântica no HTML refere-se ao uso adequado das tags para expressar o significado e a estrutura do conteúdo. As tags semânticas fornecem informações valiosas aos mecanismos de busca, leitores de tela e outros dispositivos assistivos sobre a hierarquia e a natureza do conteúdo. Isso é crucial para a acessibilidade web e para melhorar a indexação e a classificação do conteúdo pelos motores de busca. Ao utilizar tags genéricas em excesso nos componentes do Bootstrap 5, a semântica do código é comprometida, dificultando a interpretação e compreensão corretas do conteúdo.

## - Redução da Complexidade do Código:

Ao refatorar as tags genéricas nos componentes do Bootstrap 5, é possível reduzir a complexidade do código HTML. As divs em excesso tornam o código menos legível e mais difícil de dar manutenção. Ao substituir essas divs por tags semânticas adequadas, o código se torna mais claro e compreensível, facilitando a localização de seções específicas e a identificação da estrutura do documento.

## - Acessibilidade:

A refatoração de tags genéricas em componentes do Bootstrap 5 contribui para a acessibilidade web. Ao utilizar tags semânticas apropriadas, como `<article>`, `<section>`, `<header>` e `<footer>`, o conteúdo se torna mais acessível para leitores de tela e outros dispositivos assistivos. Essas tags fornecem informações significativas sobre a estrutura do conteúdo, permitindo uma navegação mais clara e compreensão do contexto para usuários com deficiências visuais.

A seguir, confira exemplos de refatoração de tags genéricas no componente de modal do Bootstrap 5.

## - Modal antes da refatoração:

```
<button type="button" class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#exampleModal">
  Launch demo modal
</button>

<div class="modal fade" id="exampleModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
  <div class="modal-dialog">
    <div class="modal-content">
      <div class="modal-header">
        <h1 class="modal-title fs-5" id="exampleModalLabel">Modal title</h1>
        <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
      </div>
      <div class="modal-body">
        ...
      </div>
      <div class="modal-footer">
        <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>
        <button type="button" class="btn btn-primary">Save changes</button>
      </div>
    </div>
  </div>
</div>
```

## - Modal após a refatoração:

```
<button type="button" class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#exampleModal">
  Launch demo modal
</button>

<article class="modal fade" id="exampleModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
  <div class="modal-dialog">
    <div class="modal-content">
      <header class="modal-header">
        <h1 class="modal-title fs-5" id="exampleModalLabel">Modal title</h1>
        <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
      </header>
      <section class="modal-body">
        ...
      </section>
      <footer class="modal-footer">
        <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>
        <button type="button" class="btn btn-primary">Save changes</button>
      </footer>
    </div>
  </div>
</article>
```

Repare que a tag `article` foi utilizada para envolver todo o conteúdo do modal. Ela serve para indicar um conteúdo independente na página, aplicação ou site. A tag `article` é um dos elementos semânticos introduzidos com o HTML5.

Já as tags `header` e `footer` foram utilizadas para representar o cabeçalho e o rodapé da página respectivamente. Essas tags podem ser utilizadas mais de uma vez em um documento HTML, diferente da tag `main`, que pode ser utilizada apenas uma vez.

### [Voltar ao README](../README.md)