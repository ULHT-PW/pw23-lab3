**PROGRAMAÇÃO WEB - aplicações web por perfeccionistas criativos**
 
# Lab 4: *SPA com layout responsivo baseado em Flexbox e Grid* 

## Objetivos
* Criar uma única página HTML, ao estilo das *Single Page Applications* (SPA).
* Aplicará os conceitos aprendidos de propriedades CSS, em especial flexbox e grid, assim como responsividade com media queries
* explorará os slides da aula para se familiarizar com a matéria e a assimilar para o mini-teste

## Recomendações
* Leia o enunciado todo com atenção antes de o começar a resolver para entender o que fará.
* Execute com atenção cada passo, certificando-se que implementa todos os detalhes. 
* Se tiver alguma dúvida, recorra aos slides da aula que contêm todos os conhecimentos que precisa para realizar o laboratório.
* Este laboratório deverá ser concluido antes da sua aula prática da semana de 21.3, onde será avaliado. 
* Todos estes conteúdos são conteúdos que saem na frequencia, pelo que exercite-os no laboratório para os conhecer.

## Pré-requisitos
* Deverá ter o Pycharm instalado para editar o código HTML de forma fácil.
* Deverá ter instalado o git no seu computador.


# 0. Estruturação do repositório de laboratórios

1. Clone (descarregue uma cópia) do GitHub para o seu computador o seu repositório com os laboratórios de Programação Web do GitHub:
    1. abra um processador de comandos (prima a tecla Windows e escreva `cmd` ou `Powershell`)
    2. escolha a pasta onde quer colocar o repositório (navegando com o comando `cd nome-de-pasta` para entrar numa determinada pasta)
    3. clone o seu repositório com o comando:
    ```bash
    > git clone https://github/seuUserName/pw-labs-nomeapelido-numero
    ```

2. Ainda usando a consola crie uma pasta lab4:
    ```bash
    > cd pw-labs-nomeapelido-numero
    > mkdir lab4
    ```

3. Atualize o ficheiro `index.html`, índice dos seus laboratórios, incluindo na lista dos laboratórios este novo laboratório com um hiperlink para `lab4/index.html`:
        * Laboratório 4: SPA com layout responsivo baseado em Flexbox e Grid

4. A estrutura da sua pasta `pw-labs-nomeapelido-numero` deverá ser como em baixo:
```
pw-labs-nomeapelido-numero
+-- index.php
+-- composer.json
+-- index.html
+-- lab1
+-- lab2
+-- lab3
+-- lab4
```


# 1. Capitais europeias com Flexbox

Neste laboratório criará uma única página HTML, ao estilo das *Single Page Applications* (SPA).
Observe a imagem em baixo (fonte: [kiwi.com](https://www.kiwi.com/pt))

![image](https://user-images.githubusercontent.com/42048382/158489558-8f31368d-e15b-4a32-82c8-683ac6b2b482.png)

Usando CSS flexbox (propriedade <code>display: flex</code>) crie um elemento flex que replique o layout acima. Para tal:
* crie uma pasta images para a qual extraia as imagens de capitais europeias contidas no ficheiro [ZIP](https://github.com/ULHT-PW/pw-lab4-2022/blob/main/capitais.zip) 
* defina, no elemento <code>head</code> a configuração para que o website tenha uma boa responsividade (veja [slide 9](https://moodle.ensinolusofona.pt/pluginfile.php/318343/mod_label/intro/pw-02.7-design-responsivo.pdf#page=9))
* escolha uma Google font que goste, inclua o link para esta e utilize-a em todo o website, definindo um seletor universal <code>*</code> e propriedade <code>font-family</code> (veja [slide](https://moodle.ensinolusofona.pt/pluginfile.php/318343/mod_label/intro/pw-02.5-propriedades-css.pdf#page=10))
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
* crie no topo um contentor flexbox para colocar o menu:
   * do lado esquerdo terá links (âncora) para os tópicos desta página, *cidades europeias* e *destinos de sonho*.
   * do lado direito terá um link para os labs de Programação Web (explore o [slide]())
* crie por baixo outro elemento que terá o cabeçalho, que incluirá:
   * imagem de fundo definida como <code>background-image</code> (veja o [slide 26](https://moodle.ensinolusofona.pt/pluginfile.php/318343/mod_label/intro/pw-02.5-propriedades-css.pdf#page=26))
   * título da página centrado usando flexbox, seguindo o princípio do [slide](https://moodle.ensinolusofona.pt/pluginfile.php/318343/mod_label/intro/pw-02.6-propriedades-css-flex-grid.pdf#page=9) 

# 3. Dicas para viajantes

* Crie um titulo <code>h1</code> "Dicas para viajantes".
* compile 8 dicas para viajantes (invente, pesquise na internet, ou veja por exemplo em [1](https://catracalivre.com.br/rede/10-conselhos-para-quem-quer-viajar-o-mundo/),  [2](https://billete996.aireuropa.com/pt-pt/10-dicas-fantasticas-para-viajar-sozinho/), [3](https://foradazonadeconforto.com/10-dicas-para-viajar-com-os-amigos/), [4](https://www.worldpackers.com/pt-BR/articles/como-viajar-com-pouco-dinheiro), [4](https://janelasabertas.com/2015/12/23/conselhos-de-viagem-que-servem-pra-vida/)). 
* Para cada dica deverá ter:
   * título
   * descrição curta (2 linhas)
   * Icone Google, Bootstrap ou Awesome (veja o s[slide](https://moodle.ensinolusofona.pt/pluginfile.php/318343/mod_label/intro/pw-02.5-propriedades-css.pdf#page=11)) 
* A seguir, crie um *container* flex (elemento <code>div</code> com classe *dicas*, estilizado com a propriedade <code>display: flex</code>)) com um conjunto de items (veja [slide 6](https://moodle.ensinolusofona.pt/pluginfile.php/318343/mod_label/intro/pw-02.6-propriedades-css-flex-grid.pdf#page=6))
* cada item será um div com a informação das dicas, o título num h1 e o texto num elemento p. 
* no css, configure os divs da classe dicas (<code>.dicas div</code>) com:
    * um tamanho igual para todos (propriedades width e height)
    * defina uma borda arredondada e uma sombra, semelhante às caixas das cidades.
    * um <code>padding: 10px 20px</code> para que o texto não fique colado à moldura (border)
    * cor de fundo o mesmo azul claro que usou no fundo do container anterior.

# 4. Destinos de sonho com CSS Grid responsivo
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
