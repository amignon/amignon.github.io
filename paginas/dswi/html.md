---
layout: page
title: Desenvolvimento de Software para Internet
permalink: /dswi/html
---



# **HTML**
---


- O HTML (**H**yper **T**ext **M**arkup **L**anguage - Linguagem de Marcação de Hipertexto) é a linguagem base da internet. Foi criada para ser de fácil entendimento por seres humanos e também por máquinas.

- O HTML é uma linguagem baseada em **marcação**.

  - Os elementos são marcados para mostrar quais informações a página exibe.
  - No exemplo abaixo o texto está entre duas marcações. Essas marcações são chamadas de **TAGs**. As tags são abertas e depois fechadas.
  <br/>

  ```html
  <h1>Aula de Desenvolvimento de Software para Internet</h1>
  ```

### **Estrutura Básica de um HTML**

<br/>

<div align="center">
  <img src="/paginas/img/estrutura_html.png" width="800px"/>
</div>


#### **Estrutura Básica - Tags**

```html
<html> e </html>
```

- **Definição**: Tag utilizada pelo navegador para identificar que o documento em questão trata-se de um HTML e não de texto puro. Entre `<html>` e `</html>` devem estar todas as outras tags, as informações e todo o conteúdo.

- **Atributos**: não possui.

<br/>

```html
<head> e </head>
```

- **Definição**: início e o fim do cabeçalho do documento, onde devem ser inseridas outras tags com dados e informações que não são exibidos na tela do navegador, mas utilizados por ele para fins diversos.

- **Atributos**: não possui.

<br/>

```html
<title> e </title>
```

- **Definição**: sempre contida entre `<head>` e `</head>` define o título do documento a ser exibido pela barra de títulos do navegador.

- **Atributos**: não possui.

<br/>

```html
<body> e </body>
```

- **Definição**: corpo do documento. Entre `<body>` e `</body>` está o que vai, efetivamente, ser exibido na tela do navegador.

- **Atributos**

  | Atributo       | Descrição |
  | --------       | --------- |
  | bgcolor        | cor de fundo da página. |
  | background     | define arquivo de imagem para o fundo da tela. |
  | leftmargin     | margem esquerda (em pixels) |
  | topmargin      | margem superior (em pixels) |
  | marginwidth    | margem pela largura (em pixels) |
  | marginheight   | margem pela altura (em pixels) |
  | text           | cor do texto para toda a página |
  | link           | cor dos links para toda página |
  | vlink          | cor dos links já visitados |
  | alink          | cor do link, quando selecionado |

<br/>

```html
<!-- e -->
```

- **Definição**: comentário. Pode ser inserido em qualquer parte do documento e seu conteúdo não é exibido pelo navegador. É utilizado para organizar o código, facilitando a visualização dos elementos dentro dele.

- **Atributos**: não possui.

#### Exemplos

<center>exemplo01.html</center>
```html
<html>
  <meta charset="utf-8">
  <head>
    <title>Minha Página</title>
  </head>
  <body>
    <!-- Inicio do Texto -->
    Olá Mundo!
  </body>
</html>
```

<center>exemplo02.html</center>
```html
<html>
  <meta charset="utf-8">
  <head>
    <title>Segunda Página</title>
  </head>
  <body>
    <h1>Página simples HTML</h1>
    <p>Olá Mundo! Minha segunda página HTML! </p>
    <p>Parágrafro comum.</p>
  </body>
</html>
```

#### **Link**

- Atributo *href=* define um link.
- O código abaixo aponta para um site

  ```html
  <a href="http://www.unip.br">Este é o link da UNIP</a>
  ```

- Adicionar um novo arquivo denominado `teste.html` e apontá-lo:

  ```html
  <a href="teste.html">Este é um link interno</a>
  ```

- **Observação**: As aspas podem ser " ou '(duplas ou simples).

#### **Dica**

- Ao receber uma página do servidor, o navegador armazena em uma memória denominada **cache** que é verificada se ela já foi visitada.

- Caso positivo, é apresentada a página local e o navegador não recebe a página do servidor.

- Isto é feito para econimizar tráfego de rede. Para contornar isto, abrir a página com `Ctrl+F5`.

#### **Imagens**

```html
<img src="arquivo.jpg" width="100" height="200">
```

- `<img>`: define uma imagem.
- `<map>`: define o mapeamento de uma imagem.
- `<area>`: define uma área *clicável* dentro de uma imagem.
- Atributos:

  - `src`: endereço da imagem.
  - `alt`: texto alternativo se a figura da imagem não for carregada.

#### **Outro Comandos**

- Break (nova linha)
  
  `<br/>`: é um elemento vazio e define uma nova linha.

- Linha Horizontal

  `<hr>`: apresenta uma linha horizontal.

#### **Listas**

- Listas Não Ordenadas

  - É uma lista de itens
  - São marcadas com *bullets*.
  - `<ul>`: Define uma lista não ordenada.
  - `<li>`: Define um item da lista.
  - Exemplo

  ```html
  <ul>
    <li>Café</li>
    <li>Leite</li>
  </ul>
  ```

  Resultado
  <div style="border: 1px solid;">
    <ul>
      <li>Café</li>
      <li>Leite</li>
    </ul>
  </div>

  <br/>

- Listas Ordenadas

  - É também uma lista de itens.
  - São marcadas com números.
  - `<ol>`: Define uma lista ordenada.
  - `<li>`: Define um item da lista.
  - Exemplo

  ```html
  <ol>
    <li>Café</li>
    <li>Leite</li>
  </ol>
  ```

  Resultado
  <div style="border: 1px solid;">
    <ol>
      <li>Café</li>
      <li>Leite</li>
    </ol>
  </div>

  <br/>

- Listas de Definiões

  - **Não** é uma lista de itens.
  - É uma lista de termos e explicações dos termos.
  - `<dl>`: Estabelece a definição de uma lista.
  - `<dl>`: Define um termo na definição de uma lista.
  - `<dd>`: Estabelece a descrição de um termo em uma lista de definição.
  - Exemplo:

  ```html
  <dl>
    <dt>Café</dt>
    <dd>Bebida quente preta</dd>
    <dt>Leite</dt>
    <dd>Bebida fria branca</dd>
  </dl>
  ``` 

  <style type="text/css" rel="stylesheet">
    dd { margin-left: 50px; }
    dt { margin-left: 5px;}
  </style>

  Resultado
  <div style="border: 1px solid;">
    <dl>
      <dt>Café</dt>
      <dd>Bebida quente preta</dd>
      <dt>Leite</dt>
      <dd>Bebida fria branca</dd>
    </dl>
  </div>

  <br/>

  [Exercício](#teste)



## Exercícios
---

1. Criar uma lista com a relação de disciplinas que vocês estão fazendo no momento. <a name="teste"></a>


## Resolução
---

Exercício 1

```html
<html>
  <meta charset="utf-8">
  <head>
    <title>Exercício 1</title>
  </head>
  <body>
    <h2>Lista de Disciplinas</h2>
    <ul>
      <li>Desenvolvimento de Software para Internet</li>
      <li>Empreendedorismo</li>
      <li>Gerenciamento de Projetos de Software</li>
      <li>Gestão da Qualidade</li>
      <li>Programação Orientada a Objetos II</li>
      <li>Projeto de Sistemas Orientados a Objetos</li>
      <li>Tópicos Especiais de Orientação a Objetos</li>
  </ul>
  </body>
</html>
```