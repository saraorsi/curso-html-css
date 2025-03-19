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

# CSS

## Introdução e sintaxe CSS


CSS (Cascading Style Sheets) é uma extensão do HTML que permite manipular os estilos de um documento ao dizer como elementos devem aparecer no browser.

Deste modo, o CSS define o design e permite que o website seja responsivo (que se adapte aos diferentes tamanhos de ecrã).

Uma regra em CSS é definida por um selector e por um bloco de declarações. Cada declaração é composta por uma propriedade e por um valor atribuído.

````
selector {
    propriedade1: valor1;
    propriedade2: valor2;
}
````

## Adicionar CSS
Podemos adicionar o CSS ao HTML de três formas diferentes:
- inline
- interno
- externo (preferencial)

### Inline
Directamente numa tag HTML através do atributo `style=""`.

Este método não é aconselhável pois, por uma questão de organização, devemos separar o código HTML do CSS.

````
<p style="color: blue">Texto azul</p>
````

### Interno
Através da tag `<style>` colocada no `<head>`, que permite que seja utilizada a sintaxe CSS dentro de um documento HTML.

````
<html>
  <head>
    <style>
      p {
        color: blue;
      }
    </style>
  </head>
  <body>
    <p>Texto azul</p>
  </body>
</html>
````

### Externo
Através de um ficheiro externo com a extensão `.css`, que permite separar o código CSS do documento HTML. 

O fichero CSS deve ser colocado na pasta do website e chamado pelo HTML através da tag `<link>` colocada no `<head>`. A tag `<link>` recebe o atributo `href=""`que recebe o caminho relativo do ficheiro CSS.

Exemplo se o ficheiro CSS (style.css) estiver na mesma pasta que o ficheiro HTML:

````
<head>
    <link rel="stylesheet" href="style.css">
<head>
````


## Selectores Classe e ID

Além das referências das tags podemos identificar os elementos de uma página pela sua "classe" ou "id".

### Classes
O selector "classe" seleciona todos os elementos HTML que têm o atributo `class=` com o valor referido antecido por um `.`. As classes identificam um grupo de elementos e um elemento pode ter mais do que uma classe.

`````
.azul {
  background: blue;
}
`````
`````
<div class="azul">
  Elemento com a class "azul"
</div>
<div class="azul">
  Elemento com a class "azul"
</div>
<div class="azul">
  Elemento com a class "azul"
</div>
`````

### IDs
O selector "id" é semelhante ao selector "classe" mas deve ser utilizado para seleccionar um elemento único que têm o atributo `id=` com o valor referido antecido por um `#`. Cada elemento apenas pode ter um "id". Normalmente os "ids" são utilizados para identificar a estrutura de uma página.

`````
<div id="cabecalho">
    Cabeçalho
</div>
<div id="noticias">
    Notícias
</div>
<div id="destaques">
    Destaques
</div>
<div id="agenda">
    Agenda
</div>
<div id="rodape">
    Rodapé
</div>
`````

## Principais Propriedades

### Box-model
- `width` define a largura da caixa;
- `height` define a altura da caixa;
- `margin` define o espaço à volta da caixa;
- `padding` define o espaço entre o limite da caixa e o seu conteúdo;
- `border` define a borda da caixa;
- `box-sizing` define se no calculo da altura e da largura estão incluídas as bordas e o padding;

### Formatacão de texto
- `font-family` altera a fonte;
- `font-size` define a altura da fonte;
- `font-weight` define o peso da fonte;
- `line-height` define a altura da linha de texto;
- `text-align` – define o alinhamento do texto (left, right, center);
- `text-decoration` – adiciona elementos decorativos ao texto;
- `text-transform` – define a capitalização do texto;
- `letter-spacing` – espaço entre os caracteres.

### Posições
A propriedade posição define o modo como um elemento é posicionado.

- `position: static;` posição relativa ao flow da página (posição por defeito);
- `position: relative;` posição relativa à sua normal posição;
- `position: absolute;`  posição relativa ao elemento pai;
- `position: fixed;`  posição relativa à viewport;
- `position: sticky;` posição relativa à posição do scroll;

### Pseudo-classes
As pseudo-classes servem para atribuir estilos consoante o estado ou a posição de um elemento.

- `:hover` `:focus` `:active` alteram consoante a interação do utilizador com determinado elementos;
- `:link` `:visited` alteram consoante a navegação;
- `:first-child` `:last-child` `:nth-child()` `:nth-last-child()` alteram consoante a posição relativa do elemento;
- `:not()` exclui os estilos desse elemento;

## Unidades

### Absolutas

As unidades absolutas têm sempre o mesmo tamanho independemente do tamanho da janela ou do elemento pai. São utilizadas quando os projectos não precisam de ser responsíveis, isto é, que não se adaptem a diferentes tamanhos de ecrã.

#### Principais unidades absolutas
Unidades Absolutas | Nome | Descrição 
--- | --- | ---
px | Pixeis | 1px = 1/96th of 1in
pt | Points | 1pt = 1/72th of 1in

### Relativas
As unidades relativas têm tamanhos escaláveis consoante o tamanho da janela ou do elemento pai. Apesar de serem um pouco mais difíceis de ser controladas, estas unidades são muito úteis para projectos que tenham de funcionar em diferentes formatados de ecrã.

#### Principais unidades relativas
Unidades Relativas | Descrição 
--- | ---
% | Percentagem relativa ao valor da propriedade no elemento pai
vw | Unidade relativa à largura da viewport. 1vw = 1/100 da largura da viewport
vh | Unidade relativa à altura da viewport. 1vh = 1/100 da altura da viewport
em | Unidade relativa ao tamanho da fonte do elemento
rem | Unidade relativa ao tamanho da fonte da root (html)

## Media Queries
As media queries servem para definir diferentes regras consoante o tipo de media ao captarem as capacidade do dispositivo. 
Assim podem identificar os seguintes valores:
- largura e altura da viewport;
- largura e altura do device;
- a orientação (horizontal ou vertical);
- a resolução.

### Sintaxe das Media Queries
````
media not|only mediatype and (expressions) {
  CSS-Code;
}
````

Valor | Descrição
--- | ---
all | Todos os tipos de media
screen | Para computadores, tablets, telemóveis, etc..
print | Para impressoras
speech | Para leitores de ecrãs

### CSS para diferentes tamanhos de ecrãs
`````
// ecrãs até 576px
@media screen and (max-width: 577px) {
 h1 {
  font-size: 20px;
 }
}
// ecrãs até 768px
@media screen and (min-width: 769px) {
 h1 {
   font-size: 15px;
 }
}
`````
