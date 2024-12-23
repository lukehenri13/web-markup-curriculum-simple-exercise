# Exercício - Curriculum com Navegação de Links, Estilização e Importação de Ícones e Web Fonte

## Objetivo

O objetivo desta atividade consiste em abordar os seguintes tópicos:

* Reconstruir uma página Web Existente
* Criar um texto com ênfase e destaque
* Criar uma imagem
* Criar um hyperlink interno e externo
* Criar uma lista não ordenada
* Criar uma lista de definição
* Criar seções com linhas horizontais
* Utilizar caracteres via entidade
* Reuso de CSS com External Stylesheet
* Declaração global de propriedades herdadas: color, font-family, font-size
* Uso do background-color para realçar regiões
* Pseudo seletores de hyperlilnk: :visited, :hover, :link, :active
* Personalizando estilo de um hyperlink
* Animações com o :hover
* Centralizando texto
* Configurar e usar fontes do Google Fonts
* Configurar e usar ícones do Material Icon e do Font Awesome
* Estilizando ícones como texto
* Valores Relativos (rem)
* CSS Media Query

## Descrição
A criação de um Curriculum Vitae é algo importante para a vida profissional. Ao saber do aumento de especialista de HTML no IFPB, algumas pessoas resolveram contratar alguém para ajudar na missão de construir um curriculum.

A princípio foi fornecido, textualmente, algumas informações que estão disponíveis com foto e algumas descrições, que juntos deverão ser apresentados em um navegador Web, conforme ilustra a Figura 1.

![](https://ifpb.github.io/exercises/_astro/layout-principal.9e289818_R97eb.png "Figura 1 - Layout do Curriculum")

Este exercício trata-se de uma continuação do exercício do Curriculo Vitae com HTML, com adição de novos recursos ao conteúdo HTML, dentre eles: o sumário com links internos, criando hiperlink entre páginas do próprio site e imagem com hiperlink.

Observe também que a estrutura do arquivo compactado é:

```
site
├── css
│   └── style.css
├── img
│   ├── avatar.png
│   └── voltar.png
├── index.html
└── pages
    └── resumo.html
```

Conforme ilustra a Figura 1 o Curriculum deve apresentar uma seção contendo, em uma lista não ordenada, um sumário com links para cada seção listada.

No index.html há uma breve descrição/resumo sobre a pessoa, no entanto uma descrição mais completa deve encontrar-se em outro documento HTML, que é acessível através do hyperlink leia mais. O conteúdo dessa segunda página deve ser conforme ilustra a Figura 2. Observe que esta possui uma imagem de uma seta que deve conter um hiperlink para o documento index.html.

![](https://ifpb.github.io/exercises/_astro/layout-resumo.ce75c4e2_1TJEcO.png "Figura 2 - Layout do Resumo")

Ainda conforme a Figura 1, no final das seções deve haver um hiperlink intitulado topo que direciona a navegação para o início do documento (index.html). Já com relação aos títulos dessas seções, devem possuir hyperlinks que recaiam para o início de sua própria seção.

Por fim, inclua no final do documento uma informação de copyright, usando entidade do HTML, conforme ilustra a Figura 1.

## Estilização
1. Para iniciar a estilização das páginas resumo.html e index.html utilize um único arquivo CSS em comum, o css/style.css.
2. Inicialmente, todo o documento deve apresentar a cor de fonte (color) com darkslategrey, o tipo de fonte (font-family) com arial, sans-serif e o tamanho de fonte (font-size) com 17px.
3. Quanto aos títulos, o h1 deve possuir tamanho de fonte de 30px, e o h2 de 24px. Além disso, o h2 deve possuir a cor de plano de fundo sendo background-color: lightskyblue; , enquanto que o h1 deve receber uma classe chamada text-center, cujo o propósito serve apenas para deixar o texto centralizado.
4. As cores de texto dos h1, h2 e a devem ser darkblue, inclusive essa cor deve ser preservada para os hyperlinks já visitados (:visited).
5. Os hyperlinks, sejam já acessados ou não, devem ser exibidos sem underline, e apenas quando o cursor do mouse estiver sobre o hyperlink é que este deverá estar com underline.
6. Em relação aos hyperlinks subjacentes aos títulos h1 e h2, visitados ou não, devem estar na cor white e lightskyblue respectivamente. Contudo, quando o cursor do mouse estiver sobre os títulos, as cores dos hyperlinks devem ser darkblue.
7. Por fim, faça que a mensagem de copyright no rodapé esteja em negrito e itálico, além disso o centralize usando a classe text-center.

## Ícones, Web Fonte e CSS Media Query
1. Aplique ao h1 a tipo de fonte Audiowide disponibilizado pelo Google, da família cursiva, e com o tamanho da fonte igual a 30px.
2. Adicione no h2 o border-radius com valor de 5px.
3. Acrescente no final do hyperlink leia mais o ícone launch do Material Icon disponibilizado pelo Google. No entanto, no documento, altere o tamanho de sua fonte para 1rem. Altere também a altura da linha do ícone e também dos parágrafos para 1.5rem.
4. No arquivo pages/resumo.html crie um botão conforme a Figura 2 composto pelo ícone arrow-circle-left, do Font Awesome disponibilizado por CDNJS, e a palavra voltar. Este botão deverá estar em um hiperlink referenciando o arquivo index.html. Internamente o botão deverá conter uma classe chamada btn, que define o tamanho de fonte de 1.3rem. Porém, quando o cursor estiver sobre este botão a cor do texto deverá ser branca, o plano de fundo darkblue e sem o sublinhado.
![](https://ifpb.github.io/exercises/_astro/button.bd5d329d_Z2aV7ge.png "Figura 3 - Aparências do botão voltar")

5. Adicione ao bloco, cujo o id é social, três hiperlinks, cada um contendo os seguintes ícones do Font Awesome: facebook-square, twitter-square, linkedin-square. Estes hiperlinks devem estar centralizados dentro do bloco, com a cor de texto branca e tamanho de fonte 2rem. Os ícones facebook-square, twitter-square, linkedin-square devem ser apresentados, respectivamente, nas cores navy, dodgerblue, navy.
6. Na visualização de impressao de ambos os documentos html:
    1. O body e o h1 devem apresentar a cor de texto preta e o tipo de fonte Times, serif;
    2. O Título h1 de id person deve estar alinhado a esquerda;
    3. O Título h2 deve possuir o plano de fundo com o valor unset;
    4. Os Hiperlinks em h2 e que os que possuem a classe topo devem possuir a cor de texto branca;