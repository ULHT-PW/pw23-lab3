# pw-lab4-2022

### Propriedades CSS
#### Fontes
* escolha e utilize uma fonte Google
* formate com todas as propriedades dos slides (font size, style, wheight, variant, e text-decoration, transform, align, leeter-spacing, word-spacing, line-height e vertical-align)

#### Icones
* utilize pelo menos 5 ícones Google, Bootstrap e Awesome 
* conte história com ícones Google

#### Cores
* explore pelo menos 3 cores "refinadas"


#### Unidades
* Faça página em que explora as unidades %, em e rem 

#### Elemento bloco e propriedades
* configure as propriedades dum conjunto de divs dentro dum contentor
* explore as propriedades background, border, width e height, padding, margin
* configure bloco de texto com figura flutuante com amrgem adequada para que texto não encoste a esta

#### Position
* explore a propriedade position e seus valores static, relative, absolute, fixed e sticky
* aplique o z-index para controlar sobreposição de elementos
* faça clip de um dos elementos


### Flex
crie uma pagina com 2 containers flex:
* cada container deverá ter 10 elementos div, o primeiro caixas de uma cor, e o segundo fotografias
* explore em cada um de forma diferente as propriedades flex-flow e justify-content e align-items.

crie um terceiro contentor, 600px de alto, com um smiley centrado no meio

### Grid
Observe o layout em baixo (fonte: [kiwi.com](https://www.kiwi.com/pt))

![Asymmetric-design](https://user-images.githubusercontent.com/42048382/158484887-93d19749-13b2-41e6-8906-f6322a668b47.jpg)

Crie uma nova página HTML e usando CSS grid (propriedade <code>display: grid</code>) crie um elemento replicando o layout encima, mas para 6 destinos em Portugal à sua escolha. Para tal, siga os seguintes passos:

#### Recolha de informação
* escolha 5 destinos em Portugal, escolhendo uma fotografia para cada um. As fotos deveráo ser redimensionadas para ser 4 quadradas e uma retangular. Escolha também uma foto alusiva a uma forma económica de férias (caravana, tenda, dormir ao relento...)

* para cada destino, defina texto de forma semelhante à imagem acima: 
    * tipo do destino
    * nome do destino
    * frase convidativa
    * tipo de destino.

### layout grid
* utilize a estruturação em grid, criando um elemento <code>div</code> com uma classe *container*, e dentro deste 6 items <code>div</code>.
* defina o layout:
   * defina para cada elemento uma classe diferente e atribua:
      *  como <code>background-image</code> uma das imagens (veja o [slide 26](https://moodle.ensinolusofona.pt/pluginfile.php/318343/mod_label/intro/pw-02.5-propriedades-css.pdf#page=26))
      *  um nome <code>grid-area</code> (veja o [slide 23](https://moodle.ensinolusofona.pt/pluginfile.php/318343/mod_label/intro/pw-02.6-propriedades-css-flex-grid.pdf#page=23))
   *  usando a propriedade <code>grid-template-areas</code> defina o layout dos elementos com as fotografias

### textos de cada foto

* Use a propriedade <code>position: relative</code> e <code>position: absolute</code> para posicionar os elementos de texto de cada fotografia como em baixo.
 
![image](https://user-images.githubusercontent.com/42048382/158486562-7b9850dc-1158-46b6-963d-ca79e059940f.png)

### Layout website
crie o layout de um website tal como indicado

### página com layout responsivo
* crie uma página com um rectangulo responsivo, na cor, ao tamanho da janela
* crie uma página com layout responsivo (PC e telemóvel)
