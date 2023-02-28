**PROGRAMAÇÃO WEB - aplicações web por perfeccionistas criativos**
 
# Lab 3: *Layouts baseados em Flexbox e Grid* 

## Objetivos
* Aplicar os conceitos aprendidos de propriedades CSS, em especial flexbox e grid.
* Criar um novo repositório e aplicação no PythonAnyWhere para este laboratório

## Recomendações
* Leia o enunciado todo com atenção antes de o começar a resolver para entender o que fará.
* Execute com atenção cada passo, certificando-se que implementa todos os detalhes. 
* Se tiver alguma dúvida, recorra aos slides da aula que contêm todos os conhecimentos que precisa para realizar o laboratório.

## Pré-requisitos
* Deverá ter o VSCode instalado para editar o código HTML de forma fácil.
* Deverá ter instalado o git no seu computador.
* reveja os slides sobre [propriedades CSS](https://moodle.ensinolusofona.pt/pluginfile.php/549222/mod_label/intro/pw-02.5-propriedades-css.pdf) e [flex e grid](https://moodle.ensinolusofona.pt/pluginfile.php/549222/mod_label/intro/pw-02.6-propriedades-css-flex-grid-short.pdf)
* explore os exercícios do tutorial [Flexbox froggy](https://flexboxfroggy.com/)

# 1. Tutoriais


# 1. Flex 

* Irá criar uma página onde explorará a propriedade <code>display:flex</code>

* escolha uma fonte Google que goste, inclua o link para esta e utilize-a em todo o website, definindo um seletor universal <code>*</code> e propriedade <code>font-family</code> (veja [slide](https://moodle.ensinolusofona.pt/pluginfile.php/318343/mod_label/intro/pw-02.5-propriedades-css.pdf#page=10))

* defina, no elemento <code>head</code> a configuração para que o website tenha uma boa responsividade (veja [slide 9](https://moodle.ensinolusofona.pt/pluginfile.php/318343/mod_label/intro/pw-02.7-design-responsivo.pdf#page=9))
* especifique no style sempre <code>* {box-sizing: border-box; padding: 0; margin: 0;}</code>

### 1.1. Elemento centrado usando <code>flex</code>

* Crie um elemento div que tenha largura 100vw e altura 50vh
* atribua-lhe uma cor de fundo
* coloque dentro do div um parágrafo <code>p</code> com a palavra 'Viajar' ou outra palavra ou frase que queira e centre-a no div, usando CSS flex (ser [slide](https://moodle.ensinolusofona.pt/pluginfile.php/549222/mod_label/intro/pw-02.6-propriedades-css-flex-grid-short.pdf#page=12)). 
* Configure o tamanho do emoji com a propriedade font-size


### 1.2. Imagem com texto usando <code>position</code>

<img src="https://user-images.githubusercontent.com/42048382/221723524-823851af-f4c9-467c-8d6f-3e3857dbbeed.png" width="300px">

* Escolha uma imagem. Pode usar o [Unsplash](https://unsplash.com/), repositório de imagems de uso livre de onde pode usar: 
   * **imagem aleatória** de acordo com termos de pesquisa e tamanho especificado. Por exemplo, para as palavras "beach sand", 600x400, especifica-se https://source.unsplash.com/random/600×400/?beach,sand. Cada vez que refrescar a sua página terá uma imagem diferente.
   * **escolher imagem**. Escolha uma imagem (das free) clique nela e copie do URL o código (unsplash.com/photos/**xg8z_KhSorQ**). Pode especificar a dimensão que pretende (e.g., 300x200). Construa o hiperlink: https://source.unsplash.com/xg8z_KhSorQ/300x200
* Crie um elemento div com <code>position:relative</code> e contendo um elemento com a imagem <code>img</code> e um elemento parágrafo <code>p</code>.
* dimensione a imagem com largura 100%, <code>width:100%</code> por forma a ocupar toda a largura do browser.
* coloque uma frase sobre a imagem usando as propriedades <code>position:absolute</code> e especificando a posição em relação ao topo <code>top</code> e lado esquerdo <code>left</code> (ver [slide](https://moodle.ensinolusofona.pt/pluginfile.php/549222/mod_label/intro/pw-02.5-propriedades-css.pdf#page=22)). EScolha uma cor para o texto que contraste bem com o fundo.


### 1.3. Capitais europeias usando <code>flex</code>

![image](https://user-images.githubusercontent.com/42048382/158489558-8f31368d-e15b-4a32-82c8-683ac6b2b482.png)

Usando uma flexbox (propriedade <code>display: flex</code>) crie um elemento flex que replique o layout acima. O código a implementar está em baixo, explicado a seguir:
* crie uma pasta images para a qual extraia as imagens de capitais europeias contidas no ficheiro [ZIP](https://github.com/ULHT-PW/pw-lab4-2022/blob/main/capitais.zip) 
* Crie um *container* flex (elemento <code>div</code> com classe *capitais*, com a propriedade <code>display: flex</code>)) e contendo um conjunto de items <code>div</code> (veja [slide 6](https://moodle.ensinolusofona.pt/pluginfile.php/549222/mod_label/intro/pw-02.6-propriedades-css-flex-grid-short.pdf#page=5))
* configure o container por forma a ter uma cor de fundo clara  (veja o [slide 11](https://moodle.ensinolusofona.pt/pluginfile.php/549222/mod_label/intro/pw-02.5-propriedades-css.pdf#page=11))
* os items serão um conjunto de elementos <code>div</code>. Cada um será alusivo a uma capital europeia tal como se descreve a seguir.
* cada item <code>div</code> deverá conter dois elementos <code>div</code>, um com a imagem, e outro com um parágrafo com o nome da capital. 
* configure os div dentro do container (recorrendo à composição de selectores <code>.container div</code>) por forma a terem uma borda e cantos arredondados (ver [slide](https://moodle.ensinolusofona.pt/pluginfile.php/549222/mod_label/intro/pw-02.5-propriedades-css.pdf#page=12))
* dentro de cada <code>div</code> coloque a imagem do lado esquerdo e do lado direito um parágrafo com o nome da cidade. para tal, configure ambos com a propriedade <code>display: inline-block</code>(ver [slide](https://moodle.ensinolusofona.pt/pluginfile.php/549222/mod_label/intro/pw-02.5-propriedades-css.pdf#page=17))
* explore as propriedades <code>flex-flow</code> e <code>justify-content</code> e <code>align-items</code> (ver [slide e links](https://moodle.ensinolusofona.pt/pluginfile.php/549222/mod_label/intro/pw-02.6-propriedades-css-flex-grid-short.pdf#page=10)) para configurar adequadamente as imagens. Garanta espaçamento entre estas, usando a propriedade <code>margin</code>. 
* Exemplo de implementação. Deverá entender em detalhe tudo o que é feito em cada selector (são conceitos que saem na frequência).

![image](https://user-images.githubusercontent.com/42048382/158496390-ad99c24c-dfe8-4030-b662-244a9eaec457.png)

### 1.4. Cabeçalho <code>header</code> com <code>position:sticky</code>

* Crie um cabeçalho, elemento <code>header</code>, fixo com a propriedade <code>position:sticky</code> (ver [codepen](https://codepen.io/LucioStuder/pen/popNbpm?editors=1100)).  
* O <code>header</code> deverá conter:
    * <code>h1</code> com um título do lado esquerdo 
    * <code>nav</code> com links "ancora" para as várias partes da página (ver [exemplo](https://moodle.ensinolusofona.pt/pluginfile.php/549222/mod_label/intro/pw-02.1-html.pdf?time=1677056603525)), e um link para uma página da próxima secção.
* O <code>header</code>, configure com <code>display:flex</code>, e faça com que o titulo e nav fiquem cada um encostado a uma lado, com a propriedade <code>justify-content:space-between</code> ([exemplo](https://codepen.io/LucioStuder/pen/oNprRQd))
* Escolha uma cor de fundo <code>background</code> e do texto <code>color</code> que goste.
* estilize os hiperlinks <code>a</code> do nav com as seguintes propriedades:
    * <code>padding:20px</code> para que haja espaço à volta de cada palavra
    * remova a formatação de hiperlink do texto (sublinhado azul), com <code>text-decoration: none</code>.
    * escolha uma cor para a fonte
    * estilize o que acontece quando passa por cima do menu. PAra tal, deverá definir o selector <code>a:hover</code> com as seguintes propriedades:
        * associe uma cor de fundo, cinza claro, quando passa por cima do link com o rato
        * texto em bold, com  <code>font-weight: bold</code>


# 2. Páginas com diferentes layouts usando <code>grid</code>
* Explore o CSS grid brincando e alterando o [codepen](https://codepen.io/LucioStuder/pen/popowOY?editors=1100). 
* O segredo do CSS grid ([slides](https://moodle.ensinolusofona.pt/pluginfile.php/549222/mod_label/intro/pw-02.6-propriedades-css-flex-grid-short.pdf#page=26)) é:
    * dar um nome <code>grid-area</code> a cada elemento do layout  
    * no contentor grid, com a propriedade <code>displaygrid</code>, caracterizar:
        * <code>grid-template-areas</code>
        * <code>grid-template-columns</code> 
        * <code>grid-template-rows</code>.
    * Explore a combinação de unidades diferentes, fr, %, vw
* Crie uma combinação de pelo menos 5 elementos semânticos HTML (header, nav, main, article, aside, footer...):
    * configure dois elementos com uma cor de fundo diferente e uma palavra a seu gosto
    * 2 com imagens de fundo (veja o [slide](https://moodle.ensinolusofona.pt/pluginfile.php/549222/mod_label/intro/pw-02.5-propriedades-css.pdf?time=1677539648106#page=5), usando  <code>background-image:url(...)</code> e <code>background-size:cover</code>). 
    * um elemento <code>grid</code>
* usando CSS grid, crie, com o mesmo conteúdo, 6 páginas com layouts diferentes, inspirando-se por exemplo [aqui](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/Design_and_accessibility/Common_web_layouts), nos layouts de 2 e 3 colunas.
* no <code>grid</code> insira 6 links (pode ser apenas um número) para cada uma das páginas, e um sexto para a página Flex. 

# 3. Submissão

1. Verifique que todos os links do seu website funcionam devidamente.
2. Crie um novo repositório GitHub público e carregue o seu laboratório 3.
3. Crie uma nova conta no pythonAnyWhere, e carregue o seu projeto
4. Verifique que o seu website online funciona corretamente, em particular mostra todas as imagens e os hiperlinks funcionam devidamente.
5. Submeta o dominio da aplicação e link do repositório GitHub.


 # Fim ☀
 
Esperamos que tenha gostado de aplicar os conhecimentos para criar layouts com flexbox e CSS grid &#127760;!
