# **Visualização de dados**
Este repositório contém os materiais utilizados nas aulas do módulo 2, no curso da Udemy.
***

# **1. O horizonte de DataViz com Python e o objetivo deste módulo**

Desde um simples gráfico de barras a um dashboard interativo, com a linguagem Python tem-se diversas ferramentas para visualização de dados e customização gráfica. Entre elas pode-se destacar as bibliotecas Matplotlib, Seaborn, Plotly, Dash.
<br><br>

Com todo esse recurso, o horizonte de possibilidades é bastante amplo. 
<br>

## **Gráficos comuns**

### Gráfico de dispersão
![image](https://github.com/lucas-mdsena/python_udemy_module_3/assets/93884007/6df57e1e-d100-4da7-8a2b-28b802092961)
<br>
### Histograma
![image](https://github.com/lucas-mdsena/python_udemy_module_3/assets/93884007/19f057eb-9c29-474e-b32f-bf6cd0683b1c)

## **Gráficos avançados**

### Gráfico de linhas sobre trabalho infantil
![image](https://github.com/lucas-mdsena/python_udemy_module_3/assets/93884007/d2258955-fc8c-4272-b0db-d9ebf6769a3f)<br>
[Fonte](https://python-graph-gallery.com/web-lineplots-and-area-chart-the-economist/)
<br>
### Gráfico lolipop mostrando as avaliações por temporada da série *The Office*
![image](https://github.com/lucas-mdsena/python_udemy_module_3/assets/93884007/3dc60a74-a7bf-4872-807a-78f7188abf4d)<br>
[Fonte](https://python-graph-gallery.com/web-lollipop-plot-with-python-the-office/)
<br>

## **Dashboards**
### [Sistema de controle de produção](https://dash.gallery/dash-manufacture-spc-dashboard/)
[Fonte](https://github.com/plotly/dash-sample-apps/tree/main/apps/dash-manufacture-spc-dashboard)
<br><br>

> Precisamos, portanto, ter um objetivo bem definido diante das possibilidades.

Com o foco do nosso curso sendo uma abordagem geral sobre a linguagem Python para análise de dados, vamos estudar, neste módulo, a criação de gráficos com a biblioteca Matplotlib, especificamente:
- Componentes de um gráfico Matplotlib;
- Abordagens de sintaxe da biblioteca;
- Escolha do tipo de gráfico adequado ao problema;
- Criação de gráficos para visualização de categorias, correlações, distribuições e evoluções;
- Boas práticas na estilização de gráficos;
- Uma pitada sobre storytelling.
<br><br>

# **2. Biblioteca Matplotlib**

[Matplotlib](https://matplotlib.org/) é uma biblioteca *open-source* desenvolvida para Python no ano de 2003, para a geração de gráficos.<br>
Uma das motivações para a criação da biblioteca foi o objetivo de oferecer a mesma usabilidade do software MATLAB, dentro do Python, por meio do módulo Pytplot (veremos isso em sequência).<br>
É uma bilbioteca que oferece grande liberdade para manipulação dos elementos de um gráfico e faz parte do arsenal para a análise de dados.
<br><br>

# **3. Componentes de um gráfico no Matplotlib**

Como dito, a biblioteca oferece grande liberdade na manipulação dos gráficos, e, para utilizarmos bem as suas ferramentas, precisamos conhecer a **anatomia das partes de um gráfico Matplotlib**.
<br>

Existem 4 elementos principais que compõem um gráficos e, de fora para dentro, podemos elencá-los:<br> 
> **Figure -> Axes -> Axis -> Artist**
<br>

- **Figure**: é a parte mais abrangente da plotagem, o quadro onde será criado um ou mais gráficos.<br>

  ![figure_intro-1](Imagens/figure_intro-1.png)
  <br>
  [Fonte](https://matplotlib.org/stable/users/explain/figure/figure_intro.html#figure-intro)
  <br>

  A região em azul na imagem é a figure, que possui apenas 1 gráfico plotado.

- **Axes**: é a parte de uma figure que contém o gráfico plotado, e uma figure pode ter vários axes. Axes possuem 2 Axis (em gráficos bidimensionais), um título, e labels para os eixos x e y.
  <br>

  ![figure_intro-1](Imagens/figure_intro-2.png)
  <br>
  [Fonte](https://matplotlib.org/stable/users/explain/figure/figure_intro.html#figure-intro)
  <br>

  A imagem acima mostra uma figure com 4 axes.

- **Axis**: são os componentes do axes que definem as escalas medidas pelo gráfico. Em plotagens bidimensionais, podemos compará-los aos eixos x e y.
- **Artist**: todos os elementos dentro de uma figure são os artist e também o que é plotado dentro de uma figure.
  <br>

  ![figure_intro-1](Imagens/anatomy.webp)
  <br>

<br><br>

# **4. Abordagens de código: Pyplot x orientação a objetos**
