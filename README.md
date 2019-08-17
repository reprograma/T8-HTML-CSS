# T8-HTML-CSS
T8 | Front-end | 2019 | Semanas 2 | Fundamentos de HTML e CSS

> Plano de aulas para a semana do dia 19/08/2019 - 23/08/2019, sobre HTML e CSS básico.
> Este arquivo será alimentado conforme o andamento das aulas 

![./github.gif]

---
## AULA 01

- [ ] Apresentação
- [ ] Combinados
- [ ] Preparando ambiente de desenvolvimento - Introdução a editores de texto
- [ ] Introdução HTML e CSS
    - [ ] O que é linguagem de marcação
    - [ ] HTML vs. HTML5
    - [ ] Elementos HTML: tags
    - [ ] Comentários no HTML
    - [ ] Adicionando links de arquivos externos  `<link>`
    - [ ] Adicionando imagens`<img>` e seus atributos `src` e `alt`)
    - [ ] O que é CSS? 
    - [ ] Diferentes formas de adicionar estilo à página 
    - [ ] Importando fontes externas (ex.: Google Fonts)
    - [ ] Estilo padrão (default) da página
    - [ ] Uso de classes e identificadores nas tags
    - [ ] Propriedades de estilo no CSS:
        - [ ] Dimensões de elementos (largura, altura)
        - [ ] Margens e espaçamentos (padding)
        - [ ] Fontes e suas cores, famílias, tamanhos e ênfases
        - [ ] Cores de fundo, transparências e gradientes
- [ ] Mãos no código
	- [ ] Exercício 01 - Landing Page Simples
	- [ ] Exercício 02 - Mini Currículo

---
## AULA 02

- [ ] Revisão de conceitos aula anterior
- [ ] Dúvidas
- [ ] Fundamentos HTML e CSS
    - [ ] Blocos`<div>`
    - [ ] Criando links `<a>` e seus atributos `href` e `target`
    - [ ] Projetando a página - wireframe
    - [ ] Hierarquia de Títulos (`<h1>` a `<h6>`)
    - [ ] Parágrafos (`<p>`)
    - [ ] Listas ordenadas e não ordenadas (`<ul>`,`<ol>` e `<li>`)
    - [ ] Tags semânticas (header, nav, footer, sections, video, article, entre outras)
    - [ ] Span 
    - [ ] Lorem ipsum (preenchendo espaços de texto)
    - [ ] Método BEM - como nomear suas classes
    - [ ] Seletores de elementos, classes e identificadores no CSS
    - [ ] Seletores por referência e pseudo seletores
    - [ ] Sobrescrita e precedência no CSS
- [ ] Mãos no código
	- [ ] Exercício - Landing Page 

---
## AULA 03

- [ ] Revisão de conceitos aula anterior
- [ ] Dúvidas
- [ ] Fundamentos HTML e CSS
    - [ ] Usando # para criar dead links
    - [ ] Links externos e links internos
    - [ ] Formulários (form, input, placeholders, checkbox, radio buttons, buttons)    
    - [ ] Propriedades de CSS
        - [ ] Bordas e sombras
        - [ ] Alinhamento de elementos
        - [ ] Propriedades display (none, block, inline, inline-block e flex)
        - [ ] Position absolute e relative
- [ ] Mãos no código
	- [ ] Exercício - Coding Dojo: form

---
## AULA 04

- [ ] Revisão de conceitos aula anterior
- [ ] Dúvidas
- [ ] Fundamentos HTML e CSS
    - [ ] Tabelas (thead, tbody, td, th e tr)
    - [ ] Propriedades de estilo no CSS:
        - [ ] Propriedade border-box
        - [ ] Cores RGB, RGBA e HEX Code
        - [ ] Medidas usadas no CSS (px, %, em e rem)
- [ ] Mãos no código
	- [ ] Exercício - Tabela

---
## AULA 05

- [ ] Revisão de conceitos aula anterior
- [ ] Dúvidas
- [ ] Fundamentos HTML e CSS
- [ ] Mãos no código
	- [ ] Exercício - Landing Page Final

---

### AULA 01 - INTRODUÇÃO À HTML E CSS

Iniciaremos com assuntos básicos de estrutura, nomenclatura e anatomia de HTML e CSS.
- [Editores de texto e organização de pastas](#editores-de-texto);
- [HTML: anatomia e introdução de tags](#html);
- [CSS: anatomia e introdução de propriedades](#css);
- [Classes, id](#classes-e-id);

#### Editores de texto
Para se modificar um arquivo .html e .css, precisamos de editor de texto. Apesar de que um simples bloco de notas pode ser a ferramenta para criação desses arquivos, vários softwares foram lançados no mercado para gostos dos programado res, oferecendo facilidades e plugins para facilitar o desenvolvimento. Alguns famosos e notáveis são:
- [Sublime Text](https://www.sublimetext.com/);
- [Notepad++](https://notepad-plus-plus.org/);
- [Atom](https://atom.io/);
- O que vamos usar durante as aulas é o [Visual Studio Code](https://code.visualstudio.com/);

A estrutura de pastas básicas é:
> css
>   style.css
> img
>   imagem.jpg
> index.html
Ou seja, uma pasta com um arquivo index.html na raiz e duas pastas: uma css para inserção de nossos estilos .css e outra img, para inserção de nossas imagens.


#### HTML
HTML é uma abreviação de **Hyper Text Markup Language** (linguagem de marcação em hipertexto). Ou seja, não se trata de uma linguagem de programação, pois não tem lógica (algoritmos, processos etc). Ele cria a **estrutura** de uma página ou aplicação web, determinando a separação de layout e seu conteúdo.

Documentos .html possuem tags de estruturação básica:
```html
<!doctype html>
<html>
    <head></head>
    <body></body>
</html>
```

Internamente, as tags html possuem uma anatomia básica também:
```html
<nome-da-tag atributo="valor do atributo">
    conteúdo
</nome-da-tag>
```

Comentários em HTML:
```html
<!-- Isso é um comentário. Comentários em qualquer linguagem são pedaços de código que são ignorados na renderização (na leitura do computador), mas são úteis para entedimento humano -->
```

#### CSS
CSS é abreviação de **Cascading Style Sheet** (folha de estilos em cascata). É a linguagem que define **estilos** para o HTML, portanto, não se trata de linguagem de programação. CSS tem "cascata" no nome, devido a sua forma de determinar a propriedade de um elemento - levando em consideração *hierarquia de seletores* e de chamadas de estilo (inline, internal e external).

Para fazer o link de um arquivo .css em um documento .html, devemos inserir a tag <link> no <head> do documento, com o href do caminho do arquivo.
```html
<!doctype html>
<html>
    <head>
        <link rel="stylesheet" href="css/style.css">
    </head>
    <body></body>
</html>
```

Dentro do arquivo .css, a anatomia é:
```css
seletor {
    propriedade: valor;
}
```

Exemplo:
```css
p {
    color: red;
}
```

Comentários em CSS:
```css
/* Sou um comentário CSS */
```


> **ATENÇÃO!**
> Não esqueçam de **indentar** o código! Isso ajuda na sua legibilidade, manutenção e colaboração com outros desenvolvedores.
> Para indentar, selecione a linha do código e aperte *tab*.

#### Classes e id
Classes e ids são atributos que podem ser inseridos em qualquer tag dentro da <body>. Eles são **atributos de nomeação**, sendo class muito usada para referência em CSS e id para Javascript (apesar de que há outras boas práticas no mercado atualmente).
Uma diferença entre os dois é que podem haver várias classes com o mesmo valor, ao passo que ids devem ser **únicos**.


#### Propriedades e tags
Verificar os arquivos de exercícios para vê-los em prática.

HTML | CSS
------------ | -------------
Tags de **estrutura**: !doctype, html, head, body | Propriedades de **background**: background-imagem, background-color
Tags no **head**: meta (charset), title, link | Propriedades de **texto**: text-align, font-family, font-size, text-decoration, font-size, text-transform
Tags de **divisão**: div | Propriedades de **layout**: width, margin, padding, display (inline-block)
Tags de **texto**: h1 ao h6, p | Propriedade de **cor**: color
Tag de **link**: a | Propriedade de **decoração**: box-shadow, border
Tag de **imagem**: img |

**Macete de centralização**: apenas para elementos block.
1. Definir um tamanho para seu elemento através da propriedade width;
2. Definir margin: 0 auto;

> O conteúdo da Aula 01 foi criado coletivamente e você pode ver o conteúdo original e completo [aqui](https://github.com/reprograma/html-css-basico#editores-de-texto)