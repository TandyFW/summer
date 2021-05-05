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