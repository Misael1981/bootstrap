# Classes do Flexbox no Bootstrap

Não é novidade que o uso de Flexbox é uma maneira poderosa de organizar o layout e dispor elementos na tela. E utilizá-lo em conjunto com o Bootstrap, é a união perfeita! Isso porque você irá gerenciar rapidamente o layout, por meio de um conjunto extremamente completo de utilitários.

## Manual do Flex no Bootstrap 5

### Flex Container

Use `d-flex` e `d-inline-flex`: para criar um container flexbox comum ou em linha e transformar os elementos filhos diretos em itens flexíveis.

### Modificando a direção

O padrão de direção no flex é `row` ou linha, então ao utilizar o Bootstrap e aplicar a classe `d-flex`, por padrão a classe `flex-row` também é aplicada. Utilize `flex-column` para definir uma direção vertical.

### Alinhamento dos itens e da caixa

### Itens Flexíveis

- **Justificando no eixo principal** (eixo x por padrão e eixo y no `flex-column` )

Use a classe `justify-content-` e em seguida aplique uma das direções que gostaria de alinhar, como por exemplo `start`,` end`,` center`,` between`,` around `ou` evenly`.

- **Alinhando no eixo cruzado (eixo y por padrão e eixo x no `flex-column`** )

Use a classe `align-items-` e assim como anteriormente, aplique uma das direções que gostaria de alinhar, como `start`,` end`,` center`,` baseline `ou` stretch`. Essa propriedade alinha de uma vez só todos os itens.

```
Caso você queira alinhar apenas 1 item flexível, você pode aplicar a classe diretamente nesse elemento e ao invés de align-items- ficará align-self-
```

## O container

Para alinhar a caixa do Flexbox em si, utilize a classe `align-content-`, somada a direção que gostaria de aplicar, ou seja, `start`,` end`,` center`,` between`,` around `ou ` stretch`.

## Capacidade de encolher e expandir

Para fazer com que um um item flexível tenha a capacidade de **crescer** para preencher o espaço disponível, utilize o utilitário `flex-grow-`, por exemplo, com `flex-grow-1` o elemento usa todo o espaço disponível, enquanto permite que os outros itens flexíveis ocupem o espaço restante.

E quando há a necessidade de fazer com que um item flexível encolha para que outro item tenha espaço, utiliza-se a classe `flex-shrink-` e o valor.

## Quebrando de linha

O padrão no flex é a ausência de quebra de linha, então ao utilizar o Bootstrap e aplicar a classe `d-flex`, por padrão a classe `flex-nowrap` também é aplicada. Caso queira que após os elementos filhos ocuparem a largura total do container, ocorra a quebra para linha de baixo, utilize o utilitário `flex-wrap`.

## Ordenando itens

É possível alterar a ordem visual de itens flexíveis específicos com a propriedade `order` do CSS, no bootstrap o utilitário também leva o mesmo nome que a propriedade somado ao valor inteiro de 0 a 5, exemplo: `order-3`.

```
Uma observação importante é que para todos os utilitários citados acima, é possível adicionar uma abreviação de breakpoint para modificar a estilização de acordo com a *responsividade. Por exemplo: .align-self-lg-start.
```

### [Voltar ao README](../README.md)