# Sintaxe de espaçamento

O Bootstrap inclui uma ampla variedade de utilitários destinados ao espaçamento, que podem ser aplicados em todos os pontos de quebra (sm, md, lg, xl e xxl).

Para aplicar a `classe` de espaçamento é bem simples, basta seguir a regra do `tipo + direção + valor`. Mas calma, vamos olhar cada um em detalhes!

## Tipo

O tipo do espaçamento indica se aquele valor que está sendo aplicado é referente ao `margin` ou ao `padding`, que são representados na classe pelas letras `m` e `p`, respectivamente.

## Direção

Uma outra informação importante que compõe a classe é pra qual lado esse espaçamento será aplicado, temos algumas opções.

- `t` significa top ou topo e é aplicado superiormente
- `b` vem de bottom e é aplicado abaixo ou inferiormente
- `s` vem de start e se refere ao left ou lado esquerdo - `do elemento
- `e` vem de end e se refere ao right ou lado direito do elemento
- `x` do eixo x ou horizontal, é aplicado à esquerda e direita do elemento
- `y` do eixo y ou vertical, é aplicado acima e abaixo do elemento
blank aplica em todos os 4 lados do elemento

## Valor

Por último, só ficou faltando dizer qual o valor que será aplicado de espaçamento, o que varia de 0 até 5 e é utilizado o rem como unidade de medida padrão.

- `0` elimina o espaçamento já definido
- `1` ou 0.25rem
- `2` ou 0.5rem
- `3` ou 1rem
- `4` ou 1.5rem
- `5` ou 3rem
- `auto` calcula automaticamente um valor para a propriedade `margin` ou `m`.

Um ponto interessante, é que ocorre um cálculo em que a variável Sass `$spacer` é multiplicada ao valor em rem da classe. Por exemplo, o `1` corresponde ao valor `$spacer` * `0.25` e isso irá ocorrer para todos os outros. Com isso, é possível modificar o valor da variável para outro valor a ser multiplicado e caso não aconteça, irá seguir o valor padrão em rem.

## Resultado final

Com esses três parâmetros a classe de espaçamento está pronta para ser utilizada, veja um exemplo abaixo.

- Aplicação no HTML

```
<h1 class="ms-1">Olá Mundo!</h1>
```

- No CSS por debaixo dos panos

```
.ms-1 {
  margin-left: ($spacer * .25) !important;
}
```

### [Voltar ao README](../README.md)
