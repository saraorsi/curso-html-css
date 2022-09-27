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

[![](https://img.youtube.com/vi/LHLtiLr6oTM/maxresdefault.jpg)](https://www.youtube.com/watch?v=LHLtiLr6oTM)

HTML (Hyper Text Markup Language) é uma linguagem de hipertexto e de marcação que descreve a estrutura de uma página web.

- Por ser uma linguagem de hipertexto aceita links que permitem o acesso directo a outras páginas.
- Por ser uma linguagem de marcação aceita `<tags>` que permitem que os browsers consigam ler de forma correcta a estrutura de um documento.

O HTML é a linguagem base do desenvolvimento web, sendo que todas as outras como o CSS, Javascript ou PHP gravitam à sua volta.

O HTML não é considerado uma linguagem de programação pois não é capaz de instruir o computador para performar operações.

Um ficheiro HTML é identificado pela extensão `.html`.

## Sintaxe do HTML

[![](https://img.youtube.com/vi/Nc1l1oZEnqs/maxresdefault.jpg)](https://www.youtube.com/watch?v=Nc1l1oZEnqs)

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

## Estrutura de um documento

[![](https://img.youtube.com/vi/uuiGQcAko0A/maxresdefault.jpg)](https://www.youtube.com/watch?v=uuiGQcAko0A)

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
