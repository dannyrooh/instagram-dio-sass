# FlexBox e Sass
## Recriando página de login do Instagram

![CSS com Super Poderes](./resources/sass.svg)


Este exemplo foi criado a partir de um desáfio do curso da [DIO](https://www.dio.me/sign-in), Recriando a página inicial do Instagram, do Bootcamp JavaScript Game Developer.


**A proposta é o aprendizado do flexbox e Sass**

<hr>

## Dependências

* Node.js
* npm

## Instalação Sass 

~~~
npm install -g sass
~~~


## VSCode

Instalar a extensão Sass

Ctrl+P
~~~
ext install sass-indented
~~~

## Build

Para transpilar seu arquivo sass em css

~~~
sass sass/style.sass css/style.css
~~~


Com o parâmetro watch ele fica observando e sempre atualizará o css
~~~
sass --watch sass/style.sass css/style.css
~~~


<hr>



# Uma breve guia de Sass, o css com super poderes

[![SASS](./resources/th.jfif)](https://sass-lang.com/)
<https://sass-lang.com/>

## Comentários
* //  não é incluso no css
* /*  incluido no css normal, não no arquivo minificado
* /*! incluido também no arquivo minificado

*obs: Está disponível nos comentário a interpolação de valores. ex: #{ 2 * 5}*


## Gerar css minificado
sass --watch sass/style.sass css/style.min.css --style copmpressed


## Nesting
"O Sass quer tornar sua vida mais fácil. Em vez de repetir os mesmos seletores repetidamente, você pode escrever regras de um estilo dentro do outro. O Sass combinará automaticamente o seletor da regra externa com o da regra interna."

https://sass-lang.com/documentation/style-rules#nesting

## Variable
"As variáveis sass são simples: você atribui um valor a um nome que começa com , e então você pode se referir a esse nome em vez do próprio valor. Mas apesar de sua simplicidade, eles são uma das ferramentas mais úteis que sass traz para a mesa. As variáveis possibilitam reduzir a repetição, fazer matemáticas complexas, configurar bibliotecas e muito mais"

https://sass-lang.com/documentation/variables

## Mixin
"Mixins permitem que você defina estilos que podem ser reutilizados em toda a sua folha de estilo. Eles facilitam o uso de aulas não semânticas como , e distribuir coleções de estilos em bibliotecas"

https://sass-lang.com/documentation/at-rules/mixin


## Extension

"Muitas vezes há casos ao projetar uma página quando uma classe deve ter todos os estilos de outra classe, bem como seus próprios estilos específicos. Por exemplo, a metodologia BEM incentiva classes de modificadores que vão nos mesmos elementos das classes de bloco ou elemento. Mas isso pode criar HTML desordenado, é propenso a erros de esquecer para incluir ambas as classes, e pode trazer preocupações de estilo não semântica em sua marcação."

https://sass-lang.com/documentation/at-rules/extend#placeholder-selectors


Em outras palavras, são padrões de estilos que outros seletores herdam.


## Import

"O Sass estende a regra @import da CSS com a capacidade de importar folhas de estilo Sass e CSS, fornecendo acesso a mixinas, funçõese variáveis e combinando várias folhas de estilo CSS juntas. Ao contrário das importações simples de CSS, que exigem que o navegador faça várias solicitações HTTP à medida que torna sua página, as importações de Sass são tratadas inteiramente durante a compilação."

https://sass-lang.com/documentation/at-rules/import