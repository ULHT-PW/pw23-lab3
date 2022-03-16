# pw-lab4-2022

# Objetivos
* Neste laboratório irá criar uma única página HTML, ao estilo das *Single Page Applications* (SPA).
* Aplicará os conceitos aprendidos de propriedades CSS, em especial flexbox e grid, assim como responsividade com media queries

# 1. Capitais europeias com Flexbox
Observe a imagem em baixo (fonte: [kiwi.com](https://www.kiwi.com/pt))

![image](https://user-images.githubusercontent.com/42048382/158489558-8f31368d-e15b-4a32-82c8-683ac6b2b482.png)

Usando CSS flexbox (propriedade <code>display: flex</code>) crie um elemento flex que replique o layout acima. Para tal:
* crie uma pasta images para a qual extraia as imagens de capitais europeias contidas no ficheiro [ZIP](https://github.com/ULHT-PW/pw-lab4-2022/blob/main/capitais.zip) 
* defina, no elemento <code>head</code> a configuração para que o website tenha uma boa responsividade (veja [slide 9](https://moodle.ensinolusofona.pt/pluginfile.php/318343/mod_label/intro/pw-02.7-design-responsivo.pdf#page=9))
* Crie um titulo <code>h1</code> "Capitais europeias".
* A seguir, crie um *container* flex (elemento <code>div</code> com classe *capitais*, estilizado com a propriedade <code>display: flex</code>)) com um conjunto de items (veja [slide 6](https://moodle.ensinolusofona.pt/pluginfile.php/318343/mod_label/intro/pw-02.6-propriedades-css-flex-grid.pdf#page=6))
* configure o container por forma a ter como cor de fundo azul muito clarinho  (veja o [slide 26](https://moodle.ensinolusofona.pt/pluginfile.php/318343/mod_label/intro/pw-02.5-propriedades-css.pdf#page=26))
* os items serão um conjunto de elementos <code>div</code>, cada um será alusivo a uma capital europeia tal como se descreve a seguir.
* cada item <code>div</code> deverá conter dois elementos <code>div</code>, um com a imagem, e outro com um parágrafo com o nome da capital. 
* configure os div dentro do container (com a composição de selectors <code>.container div</code>) por forma a terem uma borda e cantos arredondados (ver [slide](https://moodle.ensinolusofona.pt/pluginfile.php/318343/mod_label/intro/pw-02.5-propriedades-css.pdf))
* dentro de cada <code>div</code> coloque a imagem do lado esquerdo e do lado direito oum parágrafo com o nome da cidade. para tal, configure ambos com a propriedade <code>display: inline-block</code>
* explore as propriedades <code>flex-flow</code> e <code>justify-content</code> e <code>align-items</code> para configurar adequadamente as imagens. Garanta espaçamento entre estas, usando a propriedade <code>margin</code>. 
* Exemplo de implementação. Deverá entender em detalhe tudo o que é feito em cada selector (são conceitos que saem na frequência)

![image](https://user-images.githubusercontent.com/42048382/158496390-ad99c24c-dfe8-4030-b662-244a9eaec457.png)

# 2. Cabeçalho
Observe o cabeçalho em baixo do site [kiwi.com](https://www.kiwi.com/pt)).

![image](https://user-images.githubusercontent.com/42048382/158499100-5112973f-dc63-4ca6-a32c-8cd163a46b9f.png)

Crie um cabeçalho semelhante usando flexbox. Para tal:
* crie um contentor para colocar o menu:
   * do lado esquerdo terá links para cidades europeias, destinos de sonho, e do lado direito terá um link para os labs de Programação Web 
* crie por baixo outro elemento que terá o cabeçalho, que incluirá:
   * imagem de fundo definida como <code>background-image</code> (veja o [slide 26](https://moodle.ensinolusofona.pt/pluginfile.php/318343/mod_label/intro/pw-02.5-propriedades-css.pdf#page=26))
   * título da página 


# 3. Destinos de sonho com CSS Grid responsivo
Observe o layout em baixo (fonte: [kiwi.com](https://www.kiwi.com/pt))

![Asymmetric-design](https://user-images.githubusercontent.com/42048382/158484887-93d19749-13b2-41e6-8906-f6322a668b47.jpg)

Usando CSS grid (propriedade <code>display: grid</code>) crie, por debaixo do elemento anterior com cidades europeias um elemento replicando o layout encima, mas para 6 destinos em Portugal à sua escolha. Para tal, siga os seguintes passos:

#### Recolha de informação
* escolha 5 destinos em Portugal, escolhendo uma fotografia para cada um. As fotos deveráo ser redimensionadas para ser 4 quadradas e uma retangular. Escolha também uma foto alusiva a uma forma económica de férias (dormir na praia, campismo selvagem, dormir ao relento, ...).

* para cada destino, defina texto de forma semelhante à imagem acima: 
    * tipo do destino
    * nome do destino
    * frase convidativa
    * tipo de destino.

#### Configuração dos items da grid
* Crie um titulo <code>h1</code> "Destinos de sonho".
* por baixo, utilizando CSS grid, crie um elemento <code>div</code> com uma classe *destinos*, e dentro deste 6 items <code>div</code> (semelhante ao [slide 23](https://moodle.ensinolusofona.pt/pluginfile.php/318343/mod_label/intro/pw-02.6-propriedades-css-flex-grid.pdf#page=23)).
* em cada um dos 6 items <code>div</code> defina uma classe com nome específico do destino. No CSS, para cada classe:
   * defina como <code>background-image</code> a foto da do destino (veja o [slide 26](https://moodle.ensinolusofona.pt/pluginfile.php/318343/mod_label/intro/pw-02.5-propriedades-css.pdf#page=26))
   *  defina uma <code>grid-area</code> com nome da cidade (veja o [slide 23](https://moodle.ensinolusofona.pt/pluginfile.php/318343/mod_label/intro/pw-02.6-propriedades-css-flex-grid.pdf#page=23))
 
#### Layout PC 
* crie uma media query com uma regra min-width = 901px
* dentro da media query, defina a propriedade <code>grid-template-areas</code>, concebendo o layout dos items semelhante à imagem acima. Garanta algum espaçamento entre estas (propriedade <code>gap</code>).

#### Layout telemóvel
* crie uma media query com uma regra max-width = 900px
* dentro da media query, defina a propriedade <code>grid-template-areas</code>, concebendo o layout dos items d forma a que fiquem apenas duas fotos quadradas por linha. Garanta algum espaçamento entre estas (propriedade <code>gap</code>).

#### textos de cada item da foto
* Use as propriedade <code>position: relative</code> e <code>position: absolute</code> (veja o [slide 35](https://moodle.ensinolusofona.pt/pluginfile.php/318343/mod_label/intro/pw-02.5-propriedades-css.pdf#page=35)) para posicionar cada um dos 3 elementos de texto de cada fotografia como em baixo.
* escolha um tipo de fonte google giro, bastante grosso e use branco. Garanta que a foto tem contraste permitindo ler o texto.
 
![image](https://user-images.githubusercontent.com/42048382/158486562-7b9850dc-1158-46b6-963d-ca79e059940f.png)

* para o item com a sugestão de **"forma económica de férias"** (dormir na praia, campismo selvagem, dormir ao relento, ...) deverá configurar de forma semelhante à imagem inicial, com a foto na parte superior da caixa, existindo por baixo espaço branco para colocar texto (duas frases semelhantes) e um botão. Para tal, crie dentro desse div uma outra grid, com três <code>div</code>: um para a imagem (neste a imagem não fica como background), outro para a frase motivadora, e outro para o botão. 
* Para o texto (dois parágrafos) e o botão (elemento <code>button</code>, que neste caso não fará nada), cada um no seu div, deverá centrá-los de forma semelhante ao [slide 9](https://moodle.ensinolusofona.pt/pluginfile.php/318343/mod_label/intro/pw-02.6-propriedades-css-flex-grid.pdf#page=9).


# 4. Página index dos seus laboratórios
Estilize a seu gosto sua *landing page* (página de entrada) dos seus laboratórios. Em particular:
* escolha e utilize uma fonte Google
* utilize algumas propriedades dos slides (font size, style, wheight, variant, e text-decoration, transform, align, leeter-spacing, word-spacing, line-height e vertical-align)
* escolha cor de fundo
* coloque o conteúdo num conjunto de elementos semânticos (header, nav, main, footer) para organizar o conteúdo
* crie um layout CSS grid a seu gosto para organizar a informação que deverá ser responsivo à largura do ecrã (veja [slide 12](https://moodle.ensinolusofona.pt/pluginfile.php/318343/mod_label/intro/pw-02.7-design-responsivo.pdf#page=12))


#### Icones
* utilize pelo menos 5 ícones Google, Bootstrap e Awesome 
* conte história com ícones Google


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



### página com layout responsivo
* crie uma página com um rectangulo responsivo, na cor, ao tamanho da janela
* crie uma página com layout responsivo (PC e telemóvel)
