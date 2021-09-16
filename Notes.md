## Trabalhando com fontes

### Introdução font-properties

A tipografia transmite uma mensagem, por exemplo, quando queremos dar uma ênfase no texto nós podemos escrever o mesmo em negrito.

Nós podemos transmitir uma mensagem diferente dependendo do estilo que escrevemos o texto.

Algumas das propriedades de fonts do CSS que podem nos ajudar a transmitir uma mensagem através dos textos da página são:

- font-family
- font-weight
- font-style
- font-size

### Font-family

Tipo de fonte de um elemento. Essa propriedade lista as fontes em ordem de prioridade e inclui _fallback font_ (alguma fonte ou algo que vamos colocar no lugar, caso a ideia inicial não saia corretamente), como no exemplo abaixo:

```CSS
p {
  font-family: "Times New Roman", Times, serif;
}
/* o caminho ideal é imes New Roman, mas se não tiver, serve a Times; se não tiver a Times, então qualquer uma serifada  */
```

Os tipos mais comuns de fontes são com serifa e sem serifa.

### Font-weight

Peso da fonte. Seus valores:

- normal | bold | bolder | lighter | 100 | 200 | 300 | 400 | 500 | 600 | 700 | 800 | 900

Documentação para estudo: clique [aqui](https://www.w3.org/TR/css-fonts-3/).

Dependendo da família da fonte não conseguimos utilizar todos os pesos de fonte.

### Font-style

É o estilo da fonte. Seus valores são:

- normal | italic | oblique

Os valores que podem ser aplicados dependem da fonte usada, às vezes pode aceitar só o padrão normal, por exemplo.

### Font-size

É o tamanho da fonte. :)

Aceita rem (root element), px ou em (parent element), sendo os dois últimos mais comuns.

```CSS
p {
	font-size: 18px;
}
```

### Web-fonts

**Fontes do sistema x Fontes da web**

Fontes do sistema são as fontes que estão instaladas na máquina do usuário e nem sempre o cliente vai ter instalado as fontes usadas no projeto e isso pode fazer com que os estilos dos textos não sejam aplicados corretamente, mas para resolver esses casos podemos preparar nossas fonts para web ou usar fontes da web.

**Como usar fontes para web?**

- @font-face (pega fonts da nossa máquina para ser utilizada na internet, dependendo de sua extensão)
- @import (importada na tag style do HTML)
- link (maneira mais rápida para leitura de fonts)

Referências sugeridas:

- [Google Fonts](https://fonts.google.com/)
- [CSS](https://css-tricks.com/snippets/css/using-font-face/)

## Mais estilos para os textos

### Font-variant e font-stretch

1. Font-variant

Faz variações na apresentação da fonte. Os tipos podem ser vistos [aqui](https://developer.mozilla.org/en-US/docs/Web/CSS/font-variant), na documentação do Mozilla.

Exemplo:

```CSS
p {
	font-variant: small-caps;
}
```

2. Font Stretch

- Alargamento ou encolhimento da fonte;
- Aceita palavras-chaves como: expanded, condensed, normal
- Aceita porcentagens de 50% a 200%
- Essa propriedade não vai funcionar em todas as fontes.

Exemplo:

```CSS
p {
	font-stretch: expanded;
}
```

Referências:

- [font-stretch](https://developer.mozilla.org/en-US/docs/Web/CSS/font-stretch)
- [Styling_text](https://developer.mozilla.org/en-US/docs/Learn/CSS/Styling_text/Fundamentals)

### Letter e word-spacing

### Line-height e text-transform

### Text-decoration

### Text-align

### Text-shadow

### Shorthand
