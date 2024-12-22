# Exercício - Curriculum com Navegação de Links

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

## Descrição
A criação de um Curriculum Vitae é algo importante para a vida profissional. Ao saber do aumento de especialista de HTML no IFPB, algumas pessoas resolveram contratar alguém para ajudar na missão de construir um curriculum.

A princípio foi fornecido, textualmente, algumas informações que estão disponíveis com foto e algumas descrições, que juntos deverão ser apresentados em um navegador Web, conforme ilustra a Figura 1.

![](https://ifpb.github.io/exercises/_astro/layout-principal.9e289818_R97eb.png "Figura 1 - Layout do Curriculum")

Este exercício trata-se de uma continuação do exercício do Curriculo Vitae, com adição de novos recursos ao conteúdo HTML, dentre eles: o sumário com links internos, criando hiperlink entre páginas do próprio site e imagem com hiperlink.

Observe também que a estrutura do arquivo compactado é:

```
site
├── img
│   ├── avatar.jpg
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