# Entendendo container

O Bootstrap oferece uma classe chamada container que envolve o conteúdo de uma página da web, limitando sua largura máxima. Essa classe é útil para tornar o conteúdo da página legível e organizado, especialmente em dispositivos maiores onde o conteúdo pode ficar esticado e difícil de ser visualizado.

O container também é responsável por definir as margens laterais do conteúdo, alinhando e centralizando-o na página. Existem três tipos de containers no Bootstrap 5: .container, .container-fluid e .container- mais as classes de breakpoints: "`sm`", "`md`", "`lg`", "`xl`" e "`xxl`". Cada um desses containers tem uma largura diferente e pode ser usado de acordo com as necessidades do projeto.

O ".container" é o container padrão com largura fixa que se adapta a diferentes tamanhos de tela, sendo ideal para projetos que exigem controle sobre a largura do conteúdo, como páginas de produtos, por exemplo.

Exemplo abaixo:

<img src="../img/imagem5.webp">

Já o `.container-fluid` é um container que ocupa toda a largura da tela e é útil para projetos em que o conteúdo precisa ocupar toda a largura do dispositivo, como páginas de galeria de imagens ou vídeos.

Exemplo abaixo:

<img src="../img/imagem6.webp">

Por fim, o .container utilizado em conjunto com breakpoints é um container que será aplicado a partir da medida especificada pela classe de breakpoint.

No exemplo abaixo está sendo utilizada a classe `container-lg`, em uma tela com 992 pixels de largura:

<img src="../img/imagem7.webp">

Você pode conferir a largura exata em pixels que um container possui, de acordo com os pontos de quebra do bootstrap:

|             |Muito pequeno |Pequeno|	Médio|	Grande|	extra grande|	XX-Grande|
|-------------|--------------|-------|-------|--------|-------------|------------|
|             |<576px        |≥576px |≥768px |≥992 px |≥1200 px     |≥1400px     |
|.container	  |100%          |540px  |720px  |960px   |	1140px      |1320 px     |
|.container-sm|	100%	     |540px  | 720px |	960px |	1140px	    |1320 px     |
|.container-md|	100%         |100%   |	720px|	960px |	1140px      |	1320 px  |
|.container-lg|	100%         |100%   |	100% |	960px |	1140px      |	1320 px  |
|.container-xl|	100%         |	100% |	100% |	100%  |	1140px      |	1320 px  |
|.container-xxl|	100%     |	100% |	100% |	100%  |	100%        |	1320 px  |
|.container-fluid|	100%	 | 100%  |	100% |	100%  |	100%        |	100%     |


### [Voltar ao README](../README.md)
