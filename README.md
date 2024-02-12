🇧🇷 - pt-br

# Projeto "Blog vida de gato"

Por ser meu primeiro projeto utilizando animações e filtros do CSS, foi um grande desafio. Apesar das dificuldades encontradas, esse projeto fez eu perceber que tenho capacidade de aprender a programar e a prática é a chave desse aprendizado.

Apesar de simples, espero que gostem do meu projeto. Toda contribuição é bem-vinda!



## Sobre o projeto

Foi um desafio idealizado pela Rocketseat, tendo por objetivo utilizar animações e/ou filtros do CSS.



## Código

Meu objetivo foi criar animações e filtros distintos que se adequassem melhor a cada tipo de layout. Assim, ambas versões (mobile e desktop) possuem os mesmos filtros, porém as animações são distintas.

Os filtros utilizados foram *saturação, brilho e escala de cinza*.

* Filtro de saturação:
  
 ```
/*animations - just paw*/
header #paw{
    transition-property: filter;
    transition-duration: 0.6s;
}

header #paw:hover{
    filter: saturate(200%);
}

```

```
.selfie{
    width: 4.2rem;
    height: 4.2rem;
    object-fit: cover;
    border-radius: 50%;

    /*animations profile picture*/
    transition-property: filter;
    transition-duration: 0.6s;
}

.selfie:hover{
    filter: saturate(190%);
}

```

* Filtro de brilho:

```
/*animations buttons*/
#button01:hover{
    filter: brightness(1.4);
}

#button02:hover{
    filter: brightness(1.4);
}

```

* Filtro escala de cinza:

```
/*animations images*/
.item img{
    transition-property: filter;
    transition-duration: 0.6s;
}

.item img:hover{
    filter: grayscale(75%);
}

```

As animações criadas foram *appear, move e movein*.

* Para a versão mobile:

  
```
@keyframes move {
    from{
        transform: translateY(var(--startY));
    }
}


@keyframes appear {
    0% {
        opacity: 0;
        transform: scale(0.7);
    }
}

```

* Para a versão desktop:

```
 @keyframes movein {
        from{
            transform: translateX(var(--startX));
        }
    }
  ```


O tempo de duração e local de início da animação foram ajustados no CSS. Exs:

```
    main .information{
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        margin: 30px 0;

        --delay: .3s;
        --startX: -180%;
        animation: movein 1s var(--delay);
    }

    aside h1{
        --startX: 100%;
        animation: movein .6s var(--delay);
    }

    aside .item{
        --startX: 200%;
        animation: movein .6s var(--delay);
    }

```

O tempo do delay foi ajustado dentro do HTML. Exs:

```
  div class="information" style="--delay: .1s"

```


🇺🇸 - en


# "Cat life blog" project

As it was my first project using CSS animations and filters, it was a big challenge. Despite the difficulties encountered, this project made me realize that I have the ability to learn to program and practice is the key to this learning.

Although simple, I hope you like my project. Any contribution is welcome!


## About the project

It was a challenge created by Rocketseat, aiming to use animations and/or CSS filters.


## Code

My goal was to create different animations and filters that best suited each type of layout. Thus, both versions (mobile and desktop) have the same filters, but the animations are different.

The filters used were *saturation, brightness and gray scale*.

* Saturation filter:

 ```
/*animations - just paw*/
header #paw{
    transition-property: filter;
    transition-duration: 0.6s;
}

header #paw:hover{
    filter: saturate(200%);
}

```

```
.selfie{
    width: 4.2rem;
    height: 4.2rem;
    object-fit: cover;
    border-radius: 50%;

    /*animations profile picture*/
    transition-property: filter;
    transition-duration: 0.6s;
}

.selfie:hover{
    filter: saturate(190%);
}

```

* Brightness filter:

```
/*animations buttons*/
#button01:hover{
    filter: brightness(1.4);
}

#button02:hover{
    filter: brightness(1.4);
}

```

* Grayscale filter:

```
/*animations images*/
.item img{
    transition-property: filter;
    transition-duration: 0.6s;
}

.item img:hover{
    filter: grayscale(75%);
}

```

The animations created were *appear, move and movein*.

* For the mobile version:

  
```
@keyframes move {
    from{
        transform: translateY(var(--startY));
    }
}


@keyframes appear {
    0% {
        opacity: 0;
        transform: scale(0.7);
    }
}


```

* For desktop version:

 ```
 @keyframes movein {
        from{
            transform: translateX(var(--startX));
        }
    }

  ```


The duration time and start location of the animation have been adjusted in CSS. Examples:

```
    main .information{
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        margin: 30px 0;

        --delay: .3s;
        --startX: -180%;
        animation: movein 1s var(--delay);
    }

    aside h1{
        --startX: 100%;
        animation: movein .6s var(--delay);
    }

    aside .item{
        --startX: 200%;
        animation: movein .6s var(--delay);
    }

```

The delay time was adjusted within the HTML. Examples:
```
  div class="information" style="--delay: .1s"

```
