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


### Capitais europeias com Flexbox
Observe a imagem em baixo (fonte: [kiwi.com](https://www.kiwi.com/pt))

![image](https://user-images.githubusercontent.com/42048382/158489558-8f31368d-e15b-4a32-82c8-683ac6b2b482.png)

Usando CSS flexbox (propriedade <code>display: flex</code>) crie um elemento flex que replique o layout acima. Para tal:
* crie uma pasta images para a qual extraia as imagens de capitais europeias contidas no ficheiro [ZIP](https://github.com/ULHT-PW/pw-lab4-2022/blob/main/capitais.zip) 
* crie um *container* flex (elemento <code>div</code> com classe *capitais*, estilizado com a propriedade <code>display: flex</code>)) com um conjunto de items (veja [slide 6](https://moodle.ensinolusofona.pt/pluginfile.php/318343/mod_label/intro/pw-02.6-propriedades-css-flex-grid.pdf#page=6))
* configure o container por forma a ter como cor de fundo azul muito clarinho  (veja o [slide 26](https://moodle.ensinolusofona.pt/pluginfile.php/318343/mod_label/intro/pw-02.5-propriedades-css.pdf#page=26))
* os items serão um conjunto de elementos <code>div</code>, cada um será alusivo a uma capital europeia tal como se descreve a seguir.
* cada item <code>div</code> deverá conter dois elementos <code>div</code>, um com a imagem, e outro com um parágrafo com o nome da capital. 
* configure os div dentro do container (com a composição de selectors <code>.container div</code>) por forma a terem uma borda e cantos arredondados (ver [slide](https://moodle.ensinolusofona.pt/pluginfile.php/318343/mod_label/intro/pw-02.5-propriedades-css.pdf))
* dentro de cada <code>div</code> coloque a imagem do lado esquerdo e do lado direito oum parágrafo com o nome da cidade. para tal, configure ambos com a propriedade <code>display: inline-block</code>
* explore as propriedades <code>flex-flow</code> e <code>justify-content</code> e <code>align-items</code> para configurar adequadamente as imagens. Garanta espaçamento entre estas, usando a propriedade <code>margin</code>. 
* Exemplo de implementação. Deverá entender em detalhe tudo o que é feito em cada selector (são conceitos que saem na frequência)
![image](https://user-images.githubusercontent.com/42048382/158494825-72eae4e1-bbaf-4b18-a10e-439f7afe6274.png)


crie um terceiro contentor, 600px de alto, com um smiley centrado no meio

### Destinos de sonho com CSS Grid
Observe o layout em baixo (fonte: [kiwi.com](https://www.kiwi.com/pt))

![Asymmetric-design](https://user-images.githubusercontent.com/42048382/158484887-93d19749-13b2-41e6-8906-f6322a668b47.jpg)

Usando CSS grid (propriedade <code>display: grid</code>) crie um elemento replicando o layout encima, mas para 6 destinos em Portugal à sua escolha. Para tal, siga os seguintes passos:

#### Recolha de informação
* escolha 5 destinos em Portugal, escolhendo uma fotografia para cada um. As fotos deveráo ser redimensionadas para ser 4 quadradas e uma retangular. Escolha também uma foto alusiva a uma forma económica de férias (caravana, tenda, dormir ao relento...)

* para cada destino, defina texto de forma semelhante à imagem acima: 
    * tipo do destino
    * nome do destino
    * frase convidativa
    * tipo de destino.

#### layout grid
* utilize a estruturação em grid, criando um elemento <code>div</code> com uma classe *container*, e dentro deste 6 items <code>div</code>.
* defina o layout:
   * defina para cada elemento uma classe diferente e atribua:
      *  como <code>background-image</code> uma das imagens (veja o [slide 26](https://moodle.ensinolusofona.pt/pluginfile.php/318343/mod_label/intro/pw-02.5-propriedades-css.pdf#page=26))
      *  um nome para a <code>grid-area</code> (veja o [slide 23](https://moodle.ensinolusofona.pt/pluginfile.php/318343/mod_label/intro/pw-02.6-propriedades-css-flex-grid.pdf#page=23))
   *  usando a propriedade <code>grid-template-areas</code> defina o layout dos elementos com as fotografias, garantindo o espaçamento entre estas (propriedade <code>gap</code>)

#### textos de cada foto

* Use as propriedade <code>position: relative</code> e <code>position: absolute</code> (veja o [slide 35](https://moodle.ensinolusofona.pt/pluginfile.php/318343/mod_label/intro/pw-02.5-propriedades-css.pdf#page=35)) para posicionar cada um dos 3 elementos de texto de cada fotografia como em baixo.
 
![image](https://user-images.githubusercontent.com/42048382/158486562-7b9850dc-1158-46b6-963d-ca79e059940f.png)

### Layout website
crie o layout de um website tal como indicado

### página com layout responsivo
* crie uma página com um rectangulo responsivo, na cor, ao tamanho da janela
* crie uma página com layout responsivo (PC e telemóvel)
