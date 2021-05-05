# Gabarito

* Abaixo teremos uma possível solução para os exercícios propostos:

## Flexbox

### Exercício 1
Faça com que o texto e a lista fiquem um do lado do outro, o texto a esquerda da lista.

````html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    .main {
      display: flex;
      width: 50%;
    }
    .aside {

    }
    .ul {
      list-style: none;
      padding: 0;
      width: 50%;
      border: 1px solid black;
    }
  </style>
  <title>Flexbox</title>
</head>
<body>
  <main class="main">
    <section class="section">
      O Lorem Ipsum é um texto modelo da indústria tipográfica e de impressão. O Lorem Ipsum tem vindo a ser o texto padrão usado por estas indústrias desde o ano de 1500, quando uma misturou os caracteres de um texto para criar um espécime de livro. Este texto não só sobreviveu 5 séculos, mas também o salto para a tipografia electrónica, mantendo-se essencialmente inalterada. Foi popularizada nos anos 60 com a disponibilização das folhas de Letraset, que continham passagens com Lorem Ipsum, e mais recentemente com os programas de publicação como o Aldus PageMaker que incluem versões do Lorem Ipsum.
    </section>
    <aside class="aside">
      <ul class="ul">
        <li>Home</li>
        <li>Videos</li>
        <li>Pictures</li>
        <li>Leave</li>
      </ul>
    </aside>
  </main>
</body>
</html>
````

### Exercício 2
Faça com que a lista fique do lado esquerdo do texto.

````html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    .main {
      display: flex;
      flex-direction: row-reverse;
      width: 50%;
    }
    .aside {

    }
    .ul {
      list-style: none;
      padding: 0;
      width: 50%;
      border: 1px solid black;
    }
  </style>
  <title>Flexbox</title>
</head>
<body>
  <main class="main">
    <section class="section">
      O Lorem Ipsum é um texto modelo da indústria tipográfica e de impressão. O Lorem Ipsum tem vindo a ser o texto padrão usado por estas indústrias desde o ano de 1500, quando uma misturou os caracteres de um texto para criar um espécime de livro. Este texto não só sobreviveu 5 séculos, mas também o salto para a tipografia electrónica, mantendo-se essencialmente inalterada. Foi popularizada nos anos 60 com a disponibilização das folhas de Letraset, que continham passagens com Lorem Ipsum, e mais recentemente com os programas de publicação como o Aldus PageMaker que incluem versões do Lorem Ipsum.
    </section>
    <aside class="aside">
      <ul class="ul">
        <li>Home</li>
        <li>Videos</li>
        <li>Pictures</li>
        <li>Leave</li>
      </ul>
    </aside>
  </main>
</body>
</html>
````

### Exercício 3
Posicione a lista acima do texto.

````html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    .main {
      display: flex;
      flex-direction: column-reverse;
      width: 50%;
    }
    .aside {

    }
    .ul {
      list-style: none;
      padding: 0;
      width: 50%;
      border: 1px solid black;
    }
  </style>
  <title>Flexbox</title>
</head>
<body>
  <main class="main">
    <section class="section">
      O Lorem Ipsum é um texto modelo da indústria tipográfica e de impressão. O Lorem Ipsum tem vindo a ser o texto padrão usado por estas indústrias desde o ano de 1500, quando uma misturou os caracteres de um texto para criar um espécime de livro. Este texto não só sobreviveu 5 séculos, mas também o salto para a tipografia electrónica, mantendo-se essencialmente inalterada. Foi popularizada nos anos 60 com a disponibilização das folhas de Letraset, que continham passagens com Lorem Ipsum, e mais recentemente com os programas de publicação como o Aldus PageMaker que incluem versões do Lorem Ipsum.
    </section>
    <aside class="aside">
      <ul class="ul">
        <li>Home</li>
        <li>Videos</li>
        <li>Pictures</li>
        <li>Leave</li>
      </ul>
    </aside>
  </main>
</body>
</html>
````

### Exercício 4
Com a lista acima do texto, faça com que seus itens fiquem lado a lado.

````html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    .main {
      display: flex;
      flex-direction: column-reverse;
      width: 50%;
    }
    .aside {

    }
    .ul {
      display: flex;
      list-style: none;
      padding: 0;
      width: 50%;
      border: 1px solid black;
    }
  </style>
  <title>Flexbox</title>
</head>
<body>
  <main class="main">
    <section class="section">
      O Lorem Ipsum é um texto modelo da indústria tipográfica e de impressão. O Lorem Ipsum tem vindo a ser o texto padrão usado por estas indústrias desde o ano de 1500, quando uma misturou os caracteres de um texto para criar um espécime de livro. Este texto não só sobreviveu 5 séculos, mas também o salto para a tipografia electrónica, mantendo-se essencialmente inalterada. Foi popularizada nos anos 60 com a disponibilização das folhas de Letraset, que continham passagens com Lorem Ipsum, e mais recentemente com os programas de publicação como o Aldus PageMaker que incluem versões do Lorem Ipsum.
    </section>
    <aside class="aside">
      <ul class="ul">
        <li>Home</li>
        <li>Videos</li>
        <li>Pictures</li>
        <li>Leave</li>
      </ul>
    </aside>
  </main>
</body>
</html>
````

### Exercício 5
Inverta a ordem dos itens da lista.

````html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    .main {
      display: flex;
      flex-direction: column-reverse;
      width: 50%;
    }
    .aside {

    }
    .ul {
      display: flex;
      flex-direction: row-reverse;
      list-style: none;
      padding: 0;
      width: 50%;
      border: 1px solid black;
    }
  </style>
  <title>Flexbox</title>
</head>
<body>
  <main class="main">
    <section class="section">
      O Lorem Ipsum é um texto modelo da indústria tipográfica e de impressão. O Lorem Ipsum tem vindo a ser o texto padrão usado por estas indústrias desde o ano de 1500, quando uma misturou os caracteres de um texto para criar um espécime de livro. Este texto não só sobreviveu 5 séculos, mas também o salto para a tipografia electrónica, mantendo-se essencialmente inalterada. Foi popularizada nos anos 60 com a disponibilização das folhas de Letraset, que continham passagens com Lorem Ipsum, e mais recentemente com os programas de publicação como o Aldus PageMaker que incluem versões do Lorem Ipsum.
    </section>
    <aside class="aside">
      <ul class="ul">
        <li>Home</li>
        <li>Videos</li>
        <li>Pictures</li>
        <li>Leave</li>
      </ul>
    </aside>
  </main>
</body>
</html>
````

### Exercício 6
Deixe todos os itens com o mesmo espaçamento entre si e entre as bordas

````html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    .main {
      display: flex;
      flex-direction: column-reverse;
      width: 50%;
    }
    .aside {

    }
    .ul {
      display: flex;
      flex-direction: row-reverse;
      justify-content: space-evenly;
      list-style: none;
      padding: 0;
      width: 50%;
      border: 1px solid black;
    }
  </style>
  <title>Flexbox</title>
</head>
<body>
  <main class="main">
    <section class="section">
      O Lorem Ipsum é um texto modelo da indústria tipográfica e de impressão. O Lorem Ipsum tem vindo a ser o texto padrão usado por estas indústrias desde o ano de 1500, quando uma misturou os caracteres de um texto para criar um espécime de livro. Este texto não só sobreviveu 5 séculos, mas também o salto para a tipografia electrónica, mantendo-se essencialmente inalterada. Foi popularizada nos anos 60 com a disponibilização das folhas de Letraset, que continham passagens com Lorem Ipsum, e mais recentemente com os programas de publicação como o Aldus PageMaker que incluem versões do Lorem Ipsum.
    </section>
    <aside class="aside">
      <ul class="ul">
        <li>Home</li>
        <li>Videos</li>
        <li>Pictures</li>
        <li>Leave</li>
      </ul>
    </aside>
  </main>
</body>
</html>
````

### Exercício 7
Faça com que o a página fique de acordo com a imagem acima abaixo

````html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    main {
      display: flex;
      flex-direction: column;
    }
    section {
      display: flex;
      flex-flow: row wrap;
      justify-content: flex-end;
    }
    article {
      width: 40%;
    }
    ul {
      border: 1px solid black;
      display: flex;
      justify-content: space-around;
      padding: 0;
      list-style: none;
      width: 50%;
    }
    footer {
      display: flex;
      flex-direction: row-reverse;
    }
  </style>
  <title>Document</title>
</head>
<body>
  <main>
    <section>
      <article>
        <h3>O que é o Lorem Ipsum?</h3>
        <p>O Lorem Ipsum é um texto modelo da indústria tipográfica e de impressão. O Lorem Ipsum tem vindo a ser o texto padrão usado por estas indústrias desde o ano de 1500, quando uma misturou os caracteres de um texto para criar um espécime de livro. Este texto não só sobreviveu 5 séculos, mas também o salto para a tipografia electrónica, mantendo-se essencialmente inalterada. Foi popularizada nos anos 60 com a disponibilização das folhas de Letraset, que continham passagens com Lorem Ipsum, e mais recentemente com os programas de publicação como o Aldus PageMaker que incluem versões do Lorem Ipsum.</p>
      </article>
      <article>
        <h3>O que é o Lorem Ipsum?</h3>
        <p>O Lorem Ipsum é um texto modelo da indústria tipográfica e de impressão. O Lorem Ipsum tem vindo a ser o texto padrão usado por estas indústrias desde o ano de 1500, quando uma misturou os caracteres de um texto para criar um espécime de livro. Este texto não só sobreviveu 5 séculos, mas também o salto para a tipografia electrónica, mantendo-se essencialmente inalterada. Foi popularizada nos anos 60 com a disponibilização das folhas de Letraset, que continham passagens com Lorem Ipsum, e mais recentemente com os programas de publicação como o Aldus PageMaker que incluem versões do Lorem Ipsum.</p>
      </article>
      <article>
        <h3>O que é o Lorem Ipsum?</h3>
        <p>O Lorem Ipsum é um texto modelo da indústria tipográfica e de impressão. O Lorem Ipsum tem vindo a ser o texto padrão usado por estas indústrias desde o ano de 1500, quando uma misturou os caracteres de um texto para criar um espécime de livro. Este texto não só sobreviveu 5 séculos, mas também o salto para a tipografia electrónica, mantendo-se essencialmente inalterada. Foi popularizada nos anos 60 com a disponibilização das folhas de Letraset, que continham passagens com Lorem Ipsum, e mais recentemente com os programas de publicação como o Aldus PageMaker que incluem versões do Lorem Ipsum.</p>
      </article>
      <article>
        <h3>O que é o Lorem Ipsum?</h3>
        <p>O Lorem Ipsum é um texto modelo da indústria tipográfica e de impressão. O Lorem Ipsum tem vindo a ser o texto padrão usado por estas indústrias desde o ano de 1500, quando uma misturou os caracteres de um texto para criar um espécime de livro. Este texto não só sobreviveu 5 séculos, mas também o salto para a tipografia electrónica, mantendo-se essencialmente inalterada. Foi popularizada nos anos 60 com a disponibilização das folhas de Letraset, que continham passagens com Lorem Ipsum, e mais recentemente com os programas de publicação como o Aldus PageMaker que incluem versões do Lorem Ipsum.</p>
      </article>
      <article>
        <h3>O que é o Lorem Ipsum?</h3>
        <p>O Lorem Ipsum é um texto modelo da indústria tipográfica e de impressão. O Lorem Ipsum tem vindo a ser o texto padrão usado por estas indústrias desde o ano de 1500, quando uma misturou os caracteres de um texto para criar um espécime de livro. Este texto não só sobreviveu 5 séculos, mas também o salto para a tipografia electrónica, mantendo-se essencialmente inalterada. Foi popularizada nos anos 60 com a disponibilização das folhas de Letraset, que continham passagens com Lorem Ipsum, e mais recentemente com os programas de publicação como o Aldus PageMaker que incluem versões do Lorem Ipsum.</p>
      </article>
    </section>
    <footer>
      <ul>
        <li>Trabalhe conosco</li>
        <li>Sobre nós</li>
        <li>Blog</li>
      </ul>
    </footer>
  </main>
</body>
</html>
````
