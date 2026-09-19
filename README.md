# Uber Página Inicial 

Landing page inspirada na página inicial da Uber, feita para praticar HTML e Tailwind CSS. O foco deste projeto é aprender a montar uma interface responsiva usando classes utilitárias diretamente no HTML.

> Este é um projeto educacional e não é um produto oficial da Uber.

## O que você vai encontrar

- Cabeçalho com navegação;
- Seção principal com imagem de fundo e chamada para motoristas;
- Seção para empresas;
- Conteúdo sobre segurança;
- Cards informativos;
- Área de download dos aplicativos;
- Chamadas para cadastro;
- Rodapé.

## O que é Tailwind CSS?

Tailwind é um framework CSS baseado em classes pequenas e reutilizáveis. Em vez de criar uma classe CSS para cada componente, você combina classes no HTML para definir o estilo.

Por exemplo:

```html
<button class="bg-black text-white px-6 py-2 rounded-lg">
    Cadastre-se para dirigir
</button>
```

Nesse exemplo:

- `bg-black`: fundo preto;
- `text-white`: texto branco;
- `px-6`: espaço horizontal interno;
- `py-2`: espaço vertical interno;
- `rounded-lg`: bordas arredondadas.

## Conceitos de Tailwind usados neste projeto

### Layout com Flexbox

As classes `flex`, `items-center`, `justify-between` e `gap-4` organizam elementos:

```html
<div class="flex items-center justify-between gap-4">
    <!-- conteúdo -->
</div>
```

- `flex`: ativa o Flexbox;
- `items-center`: alinha os itens no centro do eixo vertical;
- `justify-between`: distribui o espaço entre os itens;
- `gap-4`: cria espaço entre os itens.

### Largura, margem e espaçamento

```html
<div class="w-full max-w-7xl mx-auto px-2">
    <!-- conteúdo centralizado -->
</div>
```

- `w-full`: ocupa toda a largura disponível;
- `max-w-7xl`: limita a largura máxima;
- `mx-auto`: centraliza horizontalmente;
- `px-2`: adiciona espaço interno dos lados.

### Responsividade

No Tailwind, um prefixo como `sm:` aplica uma classe a partir de um determinado tamanho de tela:

```html
<nav class="hidden sm:flex">
    <!-- navegação -->
</nav>
```

Nesse caso, a navegação fica escondida por padrão (`hidden`) e passa a usar Flexbox em telas maiores (`sm:flex`). O projeto também usa `md:` e `lg:` para adaptar o layout a telas médias e grandes.

### Estados de interação

O prefixo `hover:` altera o estilo quando o mouse passa sobre o elemento:

```html
<button class="hover:scale-105 duration-200">
    Começar
</button>
```

- `hover:scale-105`: aumenta levemente o botão no hover;
- `duration-200`: controla a duração da transição.

### Imagens de fundo personalizadas

No `index.html`, o bloco `@theme` cria nomes para as imagens de fundo:

```css
@theme {
    --background-image-uber: url("/assets/bguber.png");
    --background-image-city: url("/assets/bg-city.png");
}
```

Depois, essas imagens são usadas com as classes `bg-uber` e `bg-city`:

```html
<main class="bg-uber bg-no-repeat bg-cover bg-left">
```

- `bg-no-repeat`: impede a repetição da imagem;
- `bg-cover`: faz a imagem cobrir o elemento;
- `bg-left`: posiciona a imagem à esquerda.

---
![preview]()
