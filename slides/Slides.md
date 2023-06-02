---
marp: true
theme: default

style: |
  .columns {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 1rem;
  }
  .columns3 {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 1rem;
  } 
  img[alt~="center"] {
    display: block;
    margin: 0 auto;
  }
  .fa-twitter { color: aqua; }
  .fa-mastodon { color: purple; }
  .fa-linkedin { color: blue; }
  .fa-window-maximize { color: skyblue; }

  svg[id^="mermaid-"] { 
    min-width: 480px; 
    max-width: 960px; 
    min-height: 360px; 
    max-height: 600px; 
  }

  @import 'https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.3.0/css/all.min.css'
---

# Algoritmo de Floyd-Warshall

![bg right](https://picsum.photos/800/600)

---

<!-- Speaker Notes -->

## Projeto desenvolvido pelos alunos:

- Adriano Henrique
- Arom Vinicius
- Eduardo Rosalin
<!-- Can have multiple on a slide -->

---

## Algoritmo de Floyd-Warshall

O algoritmo de Floyd-Warshall é um algoritmo de programação dinâmica utilizado para encontrar os caminhos mais curtos entre todos os pares de vértices em um grafo ponderado com arestas de peso positivo ou negativo.

<!-- Can also do a multiline
comment that will show in notes -->

---

## Algoritmo de Floyd-Warshall

O algoritmo funciona criando uma matriz de distâncias entre todos os pares de vértices, onde o elemento (i, j) dessa matriz representa a menor distância entre o vértice i e o vértice j. Inicialmente, essa matriz é preenchida com as distâncias das arestas do grafo. Em seguida, o algoritmo verifica se existe um caminho de i a j passando por um vértice k com distância menor do que a distância direta entre i e j. Se houver tal caminho, a distância entre i e j é atualizada com a distância do caminho i → k → j.

---

## Algoritmo de Floyd-Warshall

O algoritmo executa essa verificação para cada par de vértices (i, j) e para cada vértice k no grafo. O algoritmo atualiza a matriz de distâncias em cada iteração, de modo que a matriz final contém as distâncias mais curtas entre todos os pares de vértices.

---

## Algoritmo de Floyd-Warshall

O algoritmo de Floyd-Warshall tem uma complexidade de tempo de O(n^3), onde n é o número de vértices no grafo. Ele é útil em muitas aplicações, como encontrar o menor caminho entre dois pontos em um mapa ou otimizar rotas em uma rede de transporte.

---

## Example:

<div class="columns">
<div>

## Grafo

## Exemplo: Grafo ponderado com arestas de peso

![width:27cm height:14cm fit](./img/grafo.jpeg)

</div>
<div>

## Exemplo: Grafo ponderado com arestas de peso

![width:27cm height:14cm fit](./img/verifica.jpeg)

</div>
</div>

---

## Slide 6

<i class="fa-brands fa-twitter"></i> Twitter:
<i class="fa-brands fa-mastodon"></i> Mastodon:
<i class="fa-brands fa-linkedin"></i> LinkedIn:
<i class="fa fa-window-maximize"></i> Blog:
<i class="fa-brands fa-github"></i> GitHub:

---

---
