<style>
  section {
    background: #fff url(./img/background.png) no-repeat center center;
    background-size: cover;
  }

  .transparent {
    background-color: transparent!important;
  }

  section.transparent img {
    background-color: transparent!important;
  }

  .transparent-table-tr-td-th {
    background-color: rgba(0, 0, 0, 0.0) !important;
  }

  .cabecalho {
    position: absolute;
    top: 10%;
    margin-left: 5%;
    margin-right: 10%;
    font-size: 48px;
    font-weight: bold;
  }

  .conteudo {
    top: 30%;
    margin-left: 5%;
    margin-right: 10%;
    font-size: 28px;
    text-align: justify;
  }

  .conteudo-absoluto {
    position: absolute;
    top: 30%;
    margin-left: 5%;
    margin-right: 10%;
    font-size: 28px;
    text-align: justify;
  }
  
  .large {
    font-size: 36px;
  }

  .normal {
    font-size: 22px;
  }
  .regular {
    font-size: 18px;
  }
  .small {
    font-size: 16px;
  }
  .footnotesize {
    font-size: 14px;
  }
  .scriptsize {
    font-size: 12px;
  }
  .tiny {
    font-size: 10px;
  }
  .bold {
    font-weight: bold;
  }
  .center {
    text-align: center;
  }
  section.lead p {
    text-align: justify;
  }
  section.lead h1 {
    text-align: center;
  }
  section.lead h2 {
    text-align: center;
  }
  
  .grid-50-50 {
    display: grid;
    grid-template-columns: 1fr 1fr;
    text-align: justify;
  }

  .grid-66-33 {
    display: grid;
    grid-template-columns: 2fr 1fr;
    text-align: justify;
  }

  .grid-33-66 {
    display: grid;
    grid-template-columns: 1fr 2fr;
    text-align: justify;
  }

  .grid-element {
    margin-left: 5%;
    margin-right: 5%;
  }
  img[alt=grid-img] {
    width: 100%;
  }
  img[alt=column-img] {
    display: block;
    margin: auto;
  }


</style>

<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>


<!-- _class: lead -->
# Análise de Circuitos Elétricos
## Aula 05 - Capacitores e Indutores

Prof. M.Sc. Diego Ascânio Santos (ascanio@cefetmg.br)

CEFET-MG DIGDDV - Divinópolis, 2023.


---

## Roteiro

1. Elementos Passivos de Armazenamento de Energia
2. Capacitores
3. Indutores
4. Combinações de Capacitores e Indutores em Série e em Paralelo
5. Indutância Mútua
6. Lista de Exercícios


---

<!-- _class: lead -->
# Elementos Passivos de Armazenamento de Energia


---

## Elementos Passivos de Armazenamento de Energia

Elementos passivos de armazenamento de energia são elementos de circuitos elétricos que, não são capazes de fornecer energia por si próprios, mas, são capazes de armazenar energia na ocasião em que uma corrente elétrica flua por eles.

São dois os elementos passivos que são capazes de armazenar energia em um circuito elétrico, sendo eles:

- [Capacitor](#05)
- [Indutor]()


---

## Capacitor

O capacitor é um componente elétrico que extrai energia de uma fonte (uma bateria por exemplo) e armazena (acumula) esta energia para libertá-la em um grande fluxo que esta fonte não seria capaz de prover. Isto ocorre porque os capacitores são capazes de acumular uma grande quantidade de carga elétrica.

![column-img](https://i.pinimg.com/originals/a2/20/ed/a220edbaef6a92efef6a7913eecb6a06.gif)




---

## Capacitor

<div class="normal">

O disparo do flash de uma câmera analógica demanda um grande fluxo de energia que uma fonte convencional não é capaz de fornecer. O capacitor, por acumular cargas, é capaz de proporcionar este fluxo, ainda que em um curtíssimo espaço de tempo.


<center>
<figure>
<img src="https://bp2.blogger.com/_1-RkxrYZ3JM/R0Y0kOvyVnI/AAAAAAAAAFc/mV_uXzjFbv8/w1200-h630-p-k-no-nu/flash+capacitor.jpg" width="40%">
<figcaption title="centered">
Capacitor em uma câmera fotográfica Cannon
</figcaption>
</figure>
</center>

</div>


---

## Capacitor

Os capacitores são amplamente utilizados em equipamentos eletrônicos e em aplicações computacionais para estabilizar tensões, filtrar sinais, acumular energia, dentre outros usos.

Apesar de armazenarem energia, não podem ser usados como baterias. Por que?

<!-- Porque os tempos em que liberam a energia armazenada são extremamente curtos, sendo incapazes de fornecer um fluxo de energia constante como o das baterias -->



---

## Capacitor

<div class="grid-50-50 normal">
<div class="grid-element">

- Frequentemente, representamos capacitores como um conjunto constituído de duas placas metálicas paralelas de área \\(A\\) separadas por um material dielétrico de largura \\(d\\) com constante de permissividade \\(\epsilon\\).

</div>
<div class="grid-element">

<!-- _class: transparent -->
![column-img](./img/capacitor.png)

</div>
</div>


---

## Capacitor

<div class="grid-50-50 regular">
<div class="grid-element">

- Quando conectamos uma fonte de tensão contínua aos terminais de um capacitor, seu terminal ligado ao pólo positivo da fonte de tensão acumula cargas \\(q\\) positivas enquanto o terminal ligado ao pólo negativo acumula cargas negativas \\(-q\\). 

- Quando o capacitor atinge seu estado estacionário (final) ele está carregado e possui uma carga total \\(q\\) diretamente proporcional à tensão \\(V\\) aplicada em seus terminais.
    - \\(q \propto V\\)

- Esta proporcionalidade pode ser mapeada por um valor \\(C\\) conhecido como capacitância do capacitor, cuja unidade de medida é o farad \\((1 F = {{1 C} \over {1 V}})\\). Assim:
\\[ q = CV \\]

</div>
<div class="grid-element">

![column-img](https://i.pinimg.com/originals/a2/20/ed/a220edbaef6a92efef6a7913eecb6a06.gif)


</div>
</div>


---

## Capacitor

<div class="grid-50-50 regular">
<div class="grid-element">

- Pela equação da carga de um capacitor \\((q = CV)\\), verificamos que a capacitância é dada pela razão entre a carga que um capacitor armazena e a diferença de potencial aplicada a seus terminais: \\(C = {{q} \over {V}}\\).

- Entretanto, a capacitância (em capacitores paralelos) não depende de \\(q\\) ou \\(v\\), mas sim, das dimensões — área \\((A)\\) das placas e a distância \\((d)\\) entre elas — e propriedades físicas — \\((\epsilon) \rightarrow \\) constante de permissividade do material dielétrico entre as placas — do capacitor, onde:

\\[C = {{\epsilon A} \over {d}}\\]

</div>
<div class="grid-element">

<!-- _class: transparent -->
![column-img](./img/capacitor.png)

</div>
</div>
