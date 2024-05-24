# Criando Badges com shields.io

[Documentação Oficial ](https://shields.io/badges/static-badge)

Não sei pra voce, mas a um primeiro momento sempre me pareceu complicado a criação dos badges. Sempre achei legal ter esses símbolos nos meus `readme.md` mas ficar procurando badges era uma tarefa complicada. Até que decidi estudar um pouco como se faz.

Sem mais delongas, vamos la.

Existem badges dos tipos dinâmicos e estáticos, aqui, abordaremos (pelo menos de momento) somente os do tipo estáticos.

Vou pular explicações e partir pra pratica pq assim tenho certeza que vc vai entender como funciona de igual forma.

## A base

`Todo` badge começa com a mesma base. Sem isso ele não funciona.

https://img.shields.io/badge/

## Notação para Markdown

Vale lembrar que a notação do markdow deve ser a seguinte:

```markdown
![seu_texto_aqui](link_pro_seu_badge)
```

Isso faz com que seu Badge apareça.

## Depois da Base Vem um Texto

Simples assim, depois da base vem textos que podem ser de diversos formatos.Nele, inclusive se definem as cores do texto exibido (a definição de cor é obrigatória).

```markdown
![](https://img.shields.io/badge/um_texto-outro_texto-blue)

```

produz:

![](https://img.shields.io/badge/um_texto-outro_texto-blue)


```markdown
![](https://img.shields.io/badge/um%20texto-outro%20texto-blue)

```

produz:

![](https://img.shields.io/badge/um%20texto-outro%20texto-blue)

## Outra Configurações

Depois do texto, temos um mundo de opções. A sequencia de opções deve ser separadas por um `?`.

Por Exemplo:

![](https://img.shields.io/badge/Meu_primeiro_badge-blue?logo=github)

Olha so quem apareceu. O logo. Eu sei que é isso que vc quer, então vamos lá.

### O logo

Os logos sao referenciados por nome e sao retirados do site : https://simpleicons.org/

Se quisermos criar um badge do git voce já sabe como fazer.

```markdow
![](https://img.shields.io/badge/Meu_primeiro_badge-blue?logo=git)

```

produz:

![](https://img.shields.io/badge/Meu_primeiro_badge-blue?logo=git)

Mas a cor do Git não é essa! Se vc pesquisar na pagina https://simpleicons.org/?q=git , vera que além do nome de referencia, tem o código na cor que é `#F05032`.
Vamos adicionar a cor sem o `#`.

```markdow
![](https://img.shields.io/badge/Meu_primeiro_badge-F05032?logo=git)

```

produz:

![](https://img.shields.io/badge/Meu_primeiro_badge-F05032?logo=git)

Mas agora ta tudo laranja! Isso mesmo mas calma, podemos escolher a cor do texto e cor do ícone.

### Adicionando Mais Opções

Toda opção posterior deve ser separada por `&`. Para Mudar a cordo da Logo faríamos:

```markdow
![](https://img.shields.io/badge/Meu_primeiro_badge-F05032?logo=git&logoColor=white)

```

produz:

![](https://img.shields.io/badge/Meu_primeiro_badge-F05032?logo=git&logoColor=white)

Vamos inverter as cores e deixar mais bonito.

```markdow
![](https://img.shields.io/badge/Meu_primeiro_badge-white?logo=git&logoColor=F05032)

```

produz:

![](https://img.shields.io/badge/Meu_primeiro_badge-white?logo=git&logoColor=F05032)

Bem melhor!

Agora vamos rápido explorar as opções.

### Style

Possible values: [flat, flat-square, plastic, for-the-badge, social]

If not specified, the default style for this badge is "flat".

#### flat

```markdow
![](https://img.shields.io/badge/Meu_primeiro_badge-white?logo=git&logoColor=F05032&style=flat)

```

produz:

![](https://img.shields.io/badge/Meu_primeiro_badge-white?logo=git&logoColor=F05032&style=flat)

#### flat-square

```markdow
![](https://img.shields.io/badge/Meu_primeiro_badge-white?logo=git&logoColor=F05032&style=flat-square)

```

produz:

![](https://img.shields.io/badge/Meu_primeiro_badge-white?logo=git&logoColor=F05032&style=flat-square)

#### plastic

```markdow
![](https://img.shields.io/badge/Meu_primeiro_badge-white?logo=git&logoColor=F05032&style=plastic)

```

produz:

![](https://img.shields.io/badge/Meu_primeiro_badge-white?logo=git&logoColor=F05032&style=plastic)

#### for-the-badge

```markdow
![](https://img.shields.io/badge/Meu_primeiro_badge-white?logo=git&logoColor=F05032&style=for-the-badge)

```

produz:

![](https://img.shields.io/badge/Meu_primeiro_badge-white?logo=git&logoColor=F05032&style=for-the-badge)

#### social

```markdow
![](https://img.shields.io/badge/Meu_primeiro_badge-white?logo=git&logoColor=F05032&style=social)

```

produz:

![](https://img.shields.io/badge/Meu_primeiro_badge-white?logo=git&logoColor=F05032&style=social)


### cacheSeconds

HTTP cache lifetime (rules are applied to infer a default value on a per-badge basis, any values specified below the default will be ignored).


```markdow
![](https://img.shields.io/badge/Meu_primeiro_badge-white?logo=git&logoColor=F05032&cacheSeconds=4000)

```

produz:

![](https://img.shields.io/badge/Meu_primeiro_badge-white?logo=git&logoColor=F05032&cacheSeconds=4000)

### Color

Background color of the right part (hex, rgb, rgba, hsl, hsla and css named colors supported).

Example: fedcba


```markdow
![](https://img.shields.io/badge/Meu_primeiro_badge-white?logo=git&logoColor=F05032&color=fedcba)

```

produz:

![](https://img.shields.io/badge/Meu_primeiro_badge-white?logo=git&logoColor=F05032&color=fedcba)


### LabelColor

Background color of the left part (hex, rgb, rgba, hsl, hsla and css named colors supported).


```markdow
![](https://img.shields.io/badge/Meu_primeiro_badge-white?logo=git&logoColor=F05032&labelcolor=abcdef)

```

produz:

![](https://img.shields.io/badge/Meu_primeiro_badge-white?logo=git&logoColor=F05032&labelcolor=abcdef)


### Label

Override the default left-hand-side text (URL-Encoding needed for spaces or special characters!)


```markdow
![](https://img.shields.io/badge/Meu_primeiro_badge-white?logo=git&logoColor=F05032&label=abcdef)

```

produz:

![](https://img.shields.io/badge/Meu_primeiro_badge-white?logo=git&logoColor=F05032&label=abcdef)


### logoSize

Make icons adaptively resize by setting auto. Useful for some wider logos like amd and amg. Supported for simple-icons logos only.

Example: auto

```markdow
![](https://img.shields.io/badge/Meu_primeiro_badge-white?logo=git&logoColor=F05032&logoSize=auto)

```

produz:

![](https://img.shields.io/badge/Meu_primeiro_badge-white?logo=git&logoColor=F05032&logoSize=auto)

### link
Specify what clicking on the left/right of a badge should do. Note that this only works when integrating your badge in an <object> HTML tag, but not an <img> tag or a markup language.

```markdow
[![](https://img.shields.io/badge/Meu_primeiro_badge-white?logo=git&logoColor=F05032)](https://github.com/blinhares)

```

produz:

[![](https://img.shields.io/badge/Meu_primeiro_badge-white?logo=git&logoColor=F05032)](https://github.com/blinhares)

## Juntando Tudo (Quase tudo...)

```![](https://img.shields.io/badge/@linhares-white?logo=git&logoColor=F05032&style=for-the-badge&label=git)```

[![](https://img.shields.io/badge/@linhares-white?logo=git&logoColor=F05032&style=for-the-badge&label=git)](https://github.com/blinhares)
