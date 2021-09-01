---
layout: page
title: Desenvolvimento de Software para Internet
permalink: /dswi/html
---

# **HTML**
---

### **Sumário**

- [Estrutura Básica de um HTML](#estrutura-basica)
- [Links](#link)
- [Imagens](#imagens)
- [Outros Comandos](#outros-comandos)
- [Listas](#listas)
- [Tabelas](#tabelas)
- [Formatações Gerais](#formatacoes)
- [Alinhamento](#alinhamento)
- [Exercícios](#exercicios)


---

- O HTML (**H**yper **T**ext **M**arkup **L**anguage - Linguagem de Marcação de Hipertexto) é a linguagem base da internet. Foi criada para ser de fácil entendimento por seres humanos e também por máquinas.

- O HTML é uma linguagem baseada em **marcação**.

  - Os elementos são marcados para mostrar quais informações a página exibe.
  - No exemplo abaixo o texto está entre duas marcações. Essas marcações são chamadas de **TAGs**. As tags são abertas e depois fechadas.
  <br/>

  ```html
  <h1>Aula de Desenvolvimento de Software para Internet</h1>
  ```

### **Estrutura Básica de um HTML** {#estrutura-basica}

<br/>

<div align="center">
  <img src="/paginas/img/estrutura_html.png" width="800px"/>
</div>

<br/>

- **Dica**: use sempre **minúsculas** nas Tags.


#### **Estrutura Básica - Tags**

```html
<!DOCTYPE html>
```
- A declaração `<!DOCTYPE html>` deve ser a primeira coisa em seu documento HTML, antes mesmo da tag `<html>`.
- O `<!DOCTYPE html>` não é uma tag HTML, é uma instrução para o navegador web sobre como interpretar o documento.

<br/>

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
<meta>
```

- A tag `<meta>`é um comando implementado no código de páginas web, dentro da área `<head>`, para passar instruções a programas externos e também para o navegador.
- Exemplo: `<meta charset="UTF-8" />`, informa ao navegador a codificação de caracteres que deve ser utilizada. 

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
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8" />
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
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8" />
    <title>Segunda Página</title>
  </head>
  <body>
    <h1>Página simples HTML</h1>
    <p>Olá Mundo! Minha segunda página HTML! </p>
    <p>Parágrafro comum.</p>
  </body>
</html>
```

#### **Links** {#link}

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

#### **Imagens** {#imagens}

```html
<img src="arquivo.jpg" width="100" height="200">
```

- `<img>`: define uma imagem.
- `<map>`: define o mapeamento de uma imagem.
- `<area>`: define uma área *clicável* dentro de uma imagem.
- Atributos:

  - `src`: endereço da imagem.
  - `alt`: texto alternativo se a figura da imagem não for carregada.

#### **Outros Comandos** {#outros-comandos}

- Break (nova linha)
  
  `<br/>`: é um elemento vazio e define uma nova linha.

- Linha Horizontal

  `<hr>`: apresenta uma linha horizontal.

#### **Listas** {#listas}

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

  <br>

  - Pode-se utilizar diferentes tipos de marcadores com as listas ordenadas, como:  `type="a"`, `type="I"` ou `type="i"`.

  ```html
  <ol type="a">
    <li> Primeiro tópico</li>
    <li> Segundo tópico</li>
  </ol>
  ```

  <br/>

- Listas de Definições

  - **Não** é uma lista de itens.
  - É uma lista de termos e explicações dos termos.
  - `<dl>`: Estabelece a definição de uma lista.
  - `<dt>`: Define um termo na definição de uma lista.
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

  [Exercício](#exercicio01)

#### **Tabelas** {#tabelas}

- Tags:

  | Tags           | Descrição |
  | --------       | --------- |
  | `<table>`      | define uma tabela. |
  | `<th>`         | define o cabeçalho de uma tabela. |
  | `<tr>`         | define a linha de uma tabela. |
  | `<td>`         | define uma célula de uma tabela. |
  | `<caption>`    | define a captura de uma tabela. |
  | `<colgroup>`   | define um grupo de colunas de uma tabela. |
  | `<col>`        | atribui valores a uma tabela |
  | `<thead>`      | define o cabeçalho de uma tabela. |
  | `<tbody>`      | define o corpo de uma tabela. |
  | `<tfoot>`      | define o rodapé de uma tabela. |

- Exemplo:

  ```html
  <!DOCTYPE html>
  <html>
    <head>
      <meta charset="utf-8">
    </head>
    <body>
      <table width="100%" border="1">
        <caption><b>Livros</b></caption>
        <tr>
          <th>ISBN</th>
          <th>Título</th>
          <th>Preço</th>
        </tr>
        <tr>
          <td>3476896</td>
          <td>Livro de HTML</td>
          <td>R$ 53,00</td>
        </tr>
        <tr>
          <td>2489604</td>
          <td>Livro de CSS</td>
          <td>R$ 47,50</td>
        </tr>
      </table>
    </body>
  </html>
  ```

  Resultado:

  <table width="100%" border="1">
    <caption><b>Livros</b></caption>
    <tr>
      <th>ISBN</th>
      <th>Título</th>
      <th>Preço</th>
    </tr>
    <tr>
      <td>3476896</td>
      <td>Livro de HTML</td>
      <td>R$ 53,00</td>
    </tr>
    <tr>
      <td>2489604</td>
      <td>Livro de CSS</td>
      <td>R$ 47,50</td>
    </tr>
  </table>

  [Exercício](#exercicio02)

#### **Formatações Gerais - Exemplo** {#formatacoes}

  - Exemplo 01: 

  ```html
  <html>
    <meta charset="utf-8">
    <head>
      <title>Trabalhando com Formatações de Texto</title>
    </head>
    <body>
      <h2>Formatações Gerais</h2>
      <hr/>
      Negrito: <b>texto</b><br>
      Itálico: <i>texto</i><br>
      Sublinhado: <u>texto</u><br>
      Riscado: <s>texto</s><br>
      Superior: <sup>texto</sup><br>
      Inferior: <sub>texto</sub><br>
      Amarelo:  <mark>texto</mark><br>
      Pequeno: <small>texto</small><br>
      Grande: <big>texto</big><br>
    </body>
  </html>
  ```

  - Resultado: 

  <div style="background-color: white; color: black; margin: 30px">
    <h2>Formatações Gerais</h2>
    <hr/>
    Negrito: <b>texto</b><br>
    Itálico: <i>texto</i><br>
    Sublinhado: <u>texto</u><br>
    Riscado: <s>texto</s><br>
    Superior: <sup>texto</sup><br>
    Inferior: <sub>texto</sub><br>
    Amarelo:  <mark>texto</mark><br>
    Pequeno: <small>texto</small><br>
    Grande: <big>texto</big><br>
  </div>

  - Exemplo 02:

  ```html
  <html>
  <meta charset="utf-8">
  <head>
    <title>Trabalhando com Formatações de Texto</title>
  </head>
    <body>
      <font color="blue" size="30" face="terminal"><p>oi</p>
      <font color="black" size="30" face="teen"><p>oi</p>
      <font color="red" size="3" face="tahoma"><p>oi</p>
      <font color="orange" size="3" face="symbol"><p>oi</p>
      <font color="green" size="13" face="pupcat"><p>oi</p>
      <font color="EE11AA" size="23" face="impact"><p>oi</p> 
      <font color="FF9600" size="3" face="arial"><p>oi</p>
    </body>
  </html> 
  ```

  - Resultado:

  <div style="background-color: white; color: black; margin: 30px">
    <font color="blue" size="30" face="terminal"><p>oi</p></font>
    <font color="black" size="30" face="teen"><p>oi</p></font>
    <font color="red" size="3" face="tahoma"><p>oi</p></font>
    <font color="orange" size="3" face="symbol"><p>oi</p></font>
    <font color="green" size="13" face="pupcat"><p>oi</p></font>
    <font color="EE11AA" size="23" face="impact"><p>oi</p> </font>
    <font color="FF9600" size="3" face="arial"><p>oi</p></font>
  </div>


#### **Alinhamento**  {#alinhamento}

  - Para deixar um texto centralizado, alinhado à esquerda ou à direita, utiliza-se os seguintes comandos:

  ```html
  <center>centraliza texto</center>
  <p align="center">centraliza texto</p>
  <p align="left">texto a esquerda</p>
  <p align="right">texto a direita</p>
  <p align="justify">texto justificado</p>
  ```

  - O atributo `align` necessita vir acompanhado de um comando principal que pode ser: `<p>`, `<br>`, `<hn>` e `<div>`.

  ```html
  <div align="right">texto a direita</div>
  ```

## Exercícios {#exercicios}
---

<div>
  <ol>
    <li>Criar uma lista com a relação de disciplinas que vocês estão fazendo no momento. <a name="exercicio01"></a></li>
    <li>Criar uma tabela com o RA e o Nome dos integrantes do seu grupo de PIM. <a name="exercicio02"></a></li>
    <li>Criar uma página HTML para representar um currículo, conforme o layout abaixo:</li>
      <br/>
      <div align="center">
        <img src="/paginas/img/html_exercicio03.png" width="800px"/>
      </div>
      <br/>
      <div style="margin-left: 20px;">
        <ul>
          <li>O Título do Navegador deve ser: <em>Currículo</em>;</li>
          <li>Usar a META TAG obrigatória de Codificação de Caracter (CHARSET);</li>
          <li>Reproduzir o Layout acima, usando Cabeçalhos, Linhas Horizontais, Listas e Parágrafos:</li>
          <li>Substituir e preencher as informações apresentadas de acordo com trajetória de cada aluno.</li>
        </ul>
      </div>
      <li>Criar uma página HTML e deixá-la com o seguinte layout. 
        <ol type="a">
          <li>O cabeçalho <em>Desenvolvimento de Sistemas</em> deve  ter tamanho 30, ficar centralizado, cor black, fonte arial.</li>
          <li>Após o cabeçalho incluir uma linha horizontal.</li>
          <li>O texto <em>Cursos de Graduação da UNIP</em> deve ser fonte Arial, tamanho 20 e cor Azul.</li>
          <li>O texto <em>Cursos de Pós-Graduação</em> deve ser Negrito, fonte Arial, tamanho 20 e cor Verde.</li>
          <li>O texto <em>Mestrado</em> deve ser Itálico, fonte Arial, tamanho 20 e cor Laranja.</li>
          <li>O texto Doutorado deve ser Sublinhado, fonte Arial, tamanho 20 e cor Vermelha.</li>
        </ol>
      </li>
      <div style="background-color: white; color: black; margin: 30px">
        <font size="30" color="black" face="arial"><p align="center">Desenvolvimento de Sistemas</p></font>
        <hr>
        <font size="20" color="blue" face="arial">Cursos de Graduação da UNIP</font><br>
        <font size="20" color="green" face="arial"><b>Cursos de Pós-Graduação</b></font><br>
        <font size="20" color="orange" face="arial"><em>Mestrado</em></font><br>
        <font size="20" color="red" face="arial"><u>Doutorado</u></font><br>
      </div>
  </ol>
</div>

  



  
  

## Resolução
---

Exercício 1

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8" />
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

Exercício 2

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
  </head>
  <body>
    <table width="100%" border="1">
      <caption><b>Grupo do PIM</b></caption>
      <tr>
        <th>RA</th>
        <th>Nome</th>
      </tr>
      <tr>
        <td>1234</td>
        <td>Ana</td>
      </tr>
      <tr>
        <td>3456</td>
        <td>João</td>
      </tr>
      <tr>
        <td>7865</td>
        <td>Matheus</td>
      </tr>
    </table>
  </body>
</html>
```