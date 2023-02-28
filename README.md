**PROGRAMAÇÃO WEB - aplicações web por perfeccionistas criativos**
 
# Lab 3: *Layouts baseados em Flexbox e Grid* 

## Objetivos
* Aplicar os conceitos aprendidos de propriedades CSS, em especial flexbox e grid.

## Recomendações
* Leia o enunciado todo com atenção antes de o começar a resolver para entender o que fará.
* Execute com atenção cada passo, certificando-se que implementa todos os detalhes. 
* Se tiver alguma dúvida, recorra aos slides da aula que contêm todos os conhecimentos que precisa para realizar o laboratório.

## Pré-requisitos
* Deverá ter o VSCode instalado para editar o código HTML de forma fácil.
* Deverá ter instalado o git no seu computador.

# 1. Tutoriais

* reveja os [slides sobre flex e grid](https://moodle.ensinolusofona.pt/pluginfile.php/549222/mod_label/intro/pw-02.6-propriedades-css-flex-grid-short.pdf)
* explore os exercícios do tutorial [Flexbox froggy](https://flexboxfroggy.com/)

# 0. Estruturação do repositório de laboratórios

1. Clone (descarregue uma cópia) do GitHub para o seu computador o seu repositório com os laboratórios de Programação Web do GitHub:
    1. abra um processador de comandos (prima a tecla Windows e escreva `cmd` ou `Powershell`)
    2. escolha a pasta onde quer colocar o repositório (navegando com o comando `cd nome-de-pasta` para entrar numa determinada pasta)
    3. clone o seu repositório com o comando:
    ```bash
    > git clone https://github/seuUserName/pw-labs-nomeapelido-numero
    ```
    

# 0. Configuração geral

* escolha uma fonte Google que goste, inclua o link para esta e utilize-a em todo o website, definindo um seletor universal <code>*</code> e propriedade <code>font-family</code> (veja [slide](https://moodle.ensinolusofona.pt/pluginfile.php/318343/mod_label/intro/pw-02.5-propriedades-css.pdf#page=10))

* defina, no elemento <code>head</code> a configuração para que o website tenha uma boa responsividade (veja [slide 9](https://moodle.ensinolusofona.pt/pluginfile.php/318343/mod_label/intro/pw-02.7-design-responsivo.pdf#page=9))

Crie uma sequência de elementos:

# 1. Elemento centrado
* Crie um elemento div que tenha largura 100vw e altura 50vh
* atribua-lhe uma cor de fundo
* coloque dentro do div um parágrafo <code><p></code> 'Viajar' ou outra palavra ou frase que queira e centre-a no div, usando CSS flex (ser [slide](https://moodle.ensinolusofona.pt/pluginfile.php/549222/mod_label/intro/pw-02.6-propriedades-css-flex-grid-short.pdf#page=12)). 
* Configure o tamanho do emoji com a propriedade font-size


# 1. Capitais europeias com Flexbox

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

# 2. Cabeçalho
Observe o cabeçalho em baixo do site [kiwi.com](https://www.kiwi.com/pt)).

![image](https://user-images.githubusercontent.com/42048382/158499100-5112973f-dc63-4ca6-a32c-8cd163a46b9f.png)

Crie um cabeçalho semelhante usando flexbox. Para tal:
* Crie no topo um contentor flexbox classe "menu" para colocar o menu:
   * do lado esquerdo terá links (âncoras) para os tópicos desta página: *cidades europeias*, *dicas para viajar* e *destinos de sonho*. do lado direito terá um link para os labs de Programação Web (ver [slide 10](https://moodle.ensinolusofona.pt/pluginfile.php/318343/mod_label/intro/pw-02.6-propriedades-css-flex-grid.pdf#page=10)). PAra criar este efeito:
       * coloque os links dentro de um container com a propriedade <code>display: flex</code>
       * configure o ultimo link, que pode identificar como <code>.menu a:last-child</code>, com a propriedade <code>margin-left:auto</code>. Isso irá encostar o último elemento à direita do container (para mais detalhes [1](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Box_Alignment/Box_Alignment_in_Flexbox#alignment_and_auto_margins))  
       * estilize o seletor <code>a</code> com as seguintes propriedades:
           * <code>padding: 20px</code> para que haja espaço à volta de cada palavra
           * remova a formatação de hiperlink do texto (sublinhado azul), com <code>text-decoration: none</code>.
           * defina uma cor à fonte
       * estilize o que acontece quando passa por cima do menu. PAra tal, deverá definir o selector <code>a:hover</code> com as seguintes propriedades:
           * associe uma cor de fundo, cinza claro, quando passa por cima do link com o rato
           * ponha o texto em bold, com  <code>font-weight: bold</code>
* Crie por baixo outro elemento que terá o cabeçalho, elemento flex que incluirá:
   * imagem de fundo definida como <code>background-image</code> desse <code>div</code> (veja o [slide 26](https://moodle.ensinolusofona.pt/pluginfile.php/318343/mod_label/intro/pw-02.5-propriedades-css.pdf#page=26))
   * título da página, dentro de um <code>div</code>, e centrado usando flexbox, seguindo o princípio do [slide](https://moodle.ensinolusofona.pt/pluginfile.php/318343/mod_label/intro/pw-02.6-propriedades-css-flex-grid.pdf#page=9) 


# 3. Dicas para viajantes

Crie um novo elemento, por baixo das cidades europeias, com dicas para viajantes. Veja um exemplo em baixo.

![image](https://user-images.githubusercontent.com/42048382/158695221-1b8a65b3-102c-4f6f-9e8a-e73f820050f7.png)

Ficará tudo na mesma página. Para tal:
* compile 8 dicas para viajantes (invente, pesquise na internet, ou veja por exemplo em [1](https://catracalivre.com.br/rede/10-conselhos-para-quem-quer-viajar-o-mundo/),  [2](https://billete996.aireuropa.com/pt-pt/10-dicas-fantasticas-para-viajar-sozinho/), [3](https://foradazonadeconforto.com/10-dicas-para-viajar-com-os-amigos/), [4](https://www.worldpackers.com/pt-BR/articles/como-viajar-com-pouco-dinheiro), [4](https://janelasabertas.com/2015/12/23/conselhos-de-viagem-que-servem-pra-vida/)). Para cada dica deverá ter:
   * título
   * descrição curta (2 linhas)
   * Icone Google, Bootstrap ou Awesome (veja o s[slide](https://moodle.ensinolusofona.pt/pluginfile.php/318343/mod_label/intro/pw-02.5-propriedades-css.pdf#page=11)) 
* Crie um titulo <code>h1</code> "Dicas para viajantes".
* Por baixo, crie um *container* flex (elemento <code>div</code> com classe *dicas*, estilizado com a propriedade <code>display: flex</code>)) com um conjunto de items (veja [slide 6](https://moodle.ensinolusofona.pt/pluginfile.php/318343/mod_label/intro/pw-02.6-propriedades-css-flex-grid.pdf#page=6)), semelhante ao exercicio anterior.
* cada item será um div com a informação das dicas, o título e ícone num h1 e o texto num elemento p. 
* no css, configure os divs da classe dicas (<code>.dicas div</code>) com:
    * um tamanho igual para todos (propriedades width e height)
    * defina uma borda arredondada e uma sombra, semelhante às caixas das cidades.
    * um <code>padding: 10px 20px</code> para que o texto não fique colado à moldura (border)
    * cor de fundo o mesmo azul claro que usou no fundo do container anterior.

# 4. Destinos de sonho com CSS Grid responsivo
Observe o layout em baixo (fonte: [kiwi.com](https://www.kiwi.com/pt))

![Asymmetric-design](https://user-images.githubusercontent.com/42048382/158484887-93d19749-13b2-41e6-8906-f6322a668b47.jpg)

Usando CSS grid (propriedade <code>display: grid</code>) crie, por debaixo do elemento anterior com dicas para viajantes um elemento replicando o layout encima, mas para 6 destinos em Portugal à sua escolha. Sim, ficará tudo na mesma página pois é uma Single Page Application (SPA). Para tal, siga os seguintes passos:

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
* o elemento destinos configure-o para que tenha como cor de fundo o mesmo azul claro que usou no fundo do container cidades. Defina tambem um padding para que os elementos não se encostem à borda da página.
* em cada um dos 6 items <code>div</code> defina uma classe com nome específico do destino. No CSS, para cada classe:
   * defina como <code>background-image</code> a foto da do destino (veja o [slide 26](https://moodle.ensinolusofona.pt/pluginfile.php/318343/mod_label/intro/pw-02.5-propriedades-css.pdf#page=26))
   *  defina uma <code>grid-area</code> com nome da cidade (veja o [slide 23](https://moodle.ensinolusofona.pt/pluginfile.php/318343/mod_label/intro/pw-02.6-propriedades-css-flex-grid.pdf#page=23))
 
#### Layout PC 
* crie uma media query com uma regra min-width = 901px
* dentro da media query, defina a propriedade <code>grid-template-areas</code>, concebendo o layout dos items semelhante à imagem acima. Garanta algum espaçamento entre estas (propriedade <code>gap</code>).

#### Layout telemóvel
* crie uma media query com uma regra max-width = 900px
* dentro da media query, defina a propriedade <code>grid-template-areas</code>, concebendo o layout dos items d forma a que fiquem apenas duas fotos quadradas por linha. Garanta algum espaçamento entre estas (propriedade <code>gap</code>).
* verifique que a responsividade funciona bem, encolhendo e alargando a página.

#### textos de cada item da foto
* Use as propriedade <code>position: relative</code> e <code>position: absolute</code> (veja o [slide 35](https://moodle.ensinolusofona.pt/pluginfile.php/318343/mod_label/intro/pw-02.5-propriedades-css.pdf#page=35)) para posicionar cada um dos 3 elementos de texto de cada fotografia como em baixo.
* escolha um tipo de fonte google giro, bastante grosso e use branco. Garanta que a foto tem contraste permitindo ler o texto.
 
![image](https://user-images.githubusercontent.com/42048382/158486562-7b9850dc-1158-46b6-963d-ca79e059940f.png)

* para o item com a sugestão de **"forma económica de férias"** (dormir na praia, campismo selvagem, dormir ao relento, ...) deverá configurar de forma semelhante à imagem inicial, com a foto na parte superior da caixa, existindo por baixo espaço branco para colocar texto (duas frases semelhantes) e um botão. Para tal, crie dentro desse div uma outra grid, com três <code>div</code>: um para a imagem (neste a imagem não fica como background), outro para a frase motivadora, e outro para o botão. 
* Para o texto (dois parágrafos) e o botão (elemento <code>button</code>, que neste caso não fará nada), cada um no seu div, deverá centrá-los de forma semelhante ao [slide 9](https://moodle.ensinolusofona.pt/pluginfile.php/318343/mod_label/intro/pw-02.6-propriedades-css-flex-grid.pdf#page=9).


# 5. Página index dos seus laboratórios
Estilize a seu gosto sua *landing page* (página de entrada) dos seus laboratórios. Em particular:
* escolha e utilize uma fonte Google
* utilize algumas propriedades dos slides (font size, style, wheight, variant, e text-decoration, transform, align, leeter-spacing, word-spacing, line-height e vertical-align)
* escolha cor de fundo
* coloque o conteúdo num conjunto de elementos semânticos (header, nav, main, footer) para organizar o conteúdo
* inclua num elemento aside uma wordcloud e posicione-a de lado (se em layout PC) ou por baixo (se em layout telemovel)
* crie um layout CSS grid a seu gosto para organizar a informação que deverá ser responsivo à largura do ecrã (veja [slide 12](https://moodle.ensinolusofona.pt/pluginfile.php/318343/mod_label/intro/pw-02.7-design-responsivo.pdf#page=12))
* utilize 5 ícones Google, Bootstrap ou Awesome (veja o s[slide](https://moodle.ensinolusofona.pt/pluginfile.php/318343/mod_label/intro/pw-02.5-propriedades-css.pdf#page=11)) 
* Explore as unidades relativas configurar o tamanho das fontes (veja o [slide](https://moodle.ensinolusofona.pt/pluginfile.php/318343/mod_label/intro/pw-02.5-propriedades-css.pdf#page=19))
* inclua um link para a nova página
 

# 6. Submissão

1. Verifique que todos os links do seu website funcionam devidamente.
2. Carregue a sua pasta do seu repositório (com as modificações efetuadas) no seu repositório Github através dos seguintes passos:
    1.  abra o processador de comandos e posicione-se dentro da pasta do seu repositório (`pw-labs-nomeapelido-numero`).
    2.  escreva as seguintes instruções:
        * `git add *`
        * `git commit –m "laboratório 4"`
        * `git push`
             * `git add` serve para propor mudaças, incluindo todos os ficheiros e pastas existentes como. o `commit` serve para confirmar as mudanças e que estas fiquem guardadas. o `push` serve para enviar as alterações (upload) para o repositório no GitHub.
3. Sincronize o GitHub com o Heroku tal como fez no [lab1](https://github.com/ULHT-PW/pw-lab1). Deverá ir ao Heroku e, em Deploy, fazer deploy branch, de forma a colocar disponível na cloud os novos conteúdos criados. 
3. Garanta que os docentes de PW são membros do seu repositório, que têm como usernames no GitHub: luciostuder, logdarkmatter, rfgsantos.
4. Verifique que o seu website online funciona corretamente, em particular mostra todas as imagens e os hiperlinks funcionam devidamente.
5. Garanta que preencheu o formulário do lab2, [form](https://forms.gle/d5sS3XtaHzRnfzQ87). Como os laboratórios estão todos centralizados num só repositório e aplicação Heroku, os docentes usarão o link submetido para avaliar os vossos trabalhos.


 # Fim ☀
 
Esperamos que tenha gostado de aplicar os conhecimentos para criar layouts com flexbox e CSS grid &#127760;!
