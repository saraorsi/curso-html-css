# Curso HTML + CSS

Curso dedicado aos princípios básicos de duas linguagens fundamentais do desenvolvimento web: HTML e CSS.

### Ferramentas necessárias:

Para este curso precisamos de instalar dois programas:

- um editor de código, que como o nome indica, serve para escrevermos o nosso código.
- um browser que ao interpretar o código, consegue renderizar, ou mostrar em tela, o nosso website com todas as suas funcionalidades.

Editor: 📥 [Visual Studio Code](https://code.visualstudio.com/)

Browser: 📥 [Chrome](https://www.google.pt/intl/pt-PT/chrome/)

### Conteúdo

- [Introdução ao HTML](#introdução-ao-html)
- [Sintaxe do HTML](#sintaxe-do-html)
- [Estrutura de um documento](#estrutura-de-um-documento)

## Introdução ao HTML

HTML (Hyper Text Markup Language) é uma linguagem de hipertexto e de marcação que descreve a estrutura de uma página web.

- Por ser uma linguagem de hipertexto aceita links que permitem o acesso directo a outras páginas.
- Por ser uma linguagem de marcação aceita `<tags>` que permitem que os browsers consigam ler de forma correcta a estrutura de um documento.

O HTML é a linguagem base do desenvolvimento web, sendo que todas as outras como o CSS, Javascript ou PHP gravitam à sua volta.

O HTML não é considerado uma linguagem de programação pois não é capaz de instruir o computador para performar operações.

Um ficheiro HTML é identificado pela extensão `.html`.

## Sintaxe do HTML

### Tags

Um documento HTML é estruturado por tags, que são os elementos que indicam como a página deve ser renderizada pelo browser.
As tags encontram-se dentro de um sinal de menor (<) e de maior (>) e, na sua maioria, têm uma marcação de início e outra de fim. Caso não tenham conteúdo as tags têm apenas uma marcação que assinala o ínicio e o fim.

```HTML
<nomeTag>Conteúdo</nomeTag> <!-- tag com conteúdo -->
<nomeTag /> <!-- tag sem conteúdo -->
```

💡 Não podemos inventar nomes para as tags. Todas as tags que existem na versão 5 do HTML encontram-se neste link: https://www.w3schools.com/TAGS/default.ASP

### Atributos

Algumas tags aceitam atributos que permitem adicionar propriedades.

```HTML
<nomeTag atributo=”valor”>Conteúdo</nomeTag>
```

💡 Também não podemos inventar atributos. Cada tag recebe determinados atributos.

### Árvore de elementos

Uma página HTML é uma estrutura que se organiza em árvore sendo que as tags podem ter pais e filhos.

```HTML
<tagParent>
    <tagChild>
    </tagChild>
</tagParent>
````

## Estrutura de um documento

Um documento HTML começa com o que chamamos de estrutura base. Esta estrutura é compostas por:

- Definição do documento (Doctype)
- Head
- Body

```HTML
<!DOCTYPE html><!-- definição do documento -->

<html>
   <head>
       <!-- No `<head>` estão as informações que não são para ser vistas em tela.  -->
   </head>

   <body>
       <!-- No `<body>` encontram-se as informações para serem apresentadas em tela. -->
   </body>
</html>
```

### Definição do documento (Doctype)

Este elemento serve para informar o browser de que se trata de um documento com código HTML. É um elemento obrigatório e deve sempre estar na primeira linha. No passado era um código longo mas na versão 5 do HTML foi simplificado para `<!DOCTYPE html>`

### Head

No `<head>` estão as informações que não são para ser vistas em tela. Nele estão os metadados, links para outros arquivos, scripts e o título do documento.

### Body

No `<body>` encontram-se as informações para serem apresentadas em tela, que podem ser em formato de texto, imagem, vídeo, áudio ou códigos embutidos.

## Primeira página

````
<!DOCTYPE html>
 
<html>
   <head>
       <title>A  minha primeira página</title> <!-- título do documento -->
       <meta charset="utf-8"> <!-- codificação da língua -->
   </head>
 
   <body>
       Olá mundo!
   </body>
</html>
````

## Tags essenciais


### Títulos e subtítulos

Os títulos e subtítulos são identificados pelas tags `<h1>` até à `<h6>`. `<h1>` o mais importante e `<h6>` menos importante.

````
<h1>Título 1</h1>
<h2>Título 2</h2>
<h3>Título 3</h3>
<h4>Título 4</h4>
<h5>Título 5</h5>
<h6>Título 6</h6>
````

### Parágrafos
Os parágrafos são identificados pela tag `<p>`.

````
<p>Isto é um parágrafo.</p>
```` 

### Lista não ordenada
Uma lista não ordenada é identificada pela tag `<ul>` e cada item pela tag `<li>`. 
Numa lista não ordenada cada item é antecedido por um símbolo bullet.

````
<ul>
    <li>Item 1</li>
    <li>Item 2</li>
    <li>Item 3</li>
</ul>
````

### Lista ordenada
Uma lista ordenada é identificada pela tag `<ol>` e cada item pela tag `<li>`. 
Numa lista ordenada cada item é numerado por ordem.

````
<ol>
    <li>Item 1</li>
    <li>Item 2</li>
    <li>Item 3</li>
</ol>
````

### Links
O links são criados utilizando a tag `<a>` que recebe o atributo `href=''` que contém o URL.

````
<a href='<!-- URL -->'>Texto que aparece</a>
````

### Imagens

As imagens são definidas pela tag `<img>` que recebe o atributo `src=''` que contém o URL da imagem ou o caminho relativo, caso a imagem esteja no nosso servidor.

````
<img width='500' src='<!-- URL da Imagem -->'>
<img width='500' src='<!-- caminho relativo -->'>
````

### Tags de Formatação de Texto
- `<b>` negrito
- `<strong>` forte
- `<i>` itálico
- `<em>` enfatizado
- `<big>` grande
- `<small>` pequeno
- `<sub>` subscrito
- `<sup>` superescrito
- `<ins>` inserido
- `<del>` cancelado
- `<u>` sublinhado [esta tag está desaprovado, recomenda-se utilizar os estilos]

````
<b>negrito</b>
<strong>forte</strong>
<i>itálico</i>
<em>enfatizado</em>
<big>grande</big>
<small>pequeno</small>
<sub>subscrito</sub>
<sup>superescrito</sup>
<ins>inserido</ins>
<del>cancelado</del>
<u>sublinhado</u>
````
