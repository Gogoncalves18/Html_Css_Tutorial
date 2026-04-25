# Anotacoes de uso deste arquivo

1. Títulos
Use o símbolo # seguido de um espaço. 
# Título 1 (Principal)
## Título 2 (Seção)
### Título 3 (Subseção)
2. Formatação de Texto
Negrito: **texto**
Itálico: *texto* ou _texto_
Riscado: ~~texto~~ 
3. Listas
Lista com marcadores: Use -, * ou +.
Lista numerada: Use 1., 2., etc.
Checklist: - [ ] Tarefa ou - [x] Concluída. 
4. Links e Imagens
Link: [Nome do Link](URL)
Imagem: ![Descrição](URL_da_imagem)
5. Blocos de Código
Para código na linha: `comando`
Para blocos grandes: use três crases (` ` `) no início e no fim. 
6. Citações e Divisores
Citação: > Texto da citação
Linha divisória: ---

---

# Curso  de HMTL e CSS Completo

## TAGS IMPORTANTES
**HEAD** - Aqui é onde é a config da pagina e nao aparece na pagina 

**html** - pega todo o arquivo html para aplicar o estilo, como classe.

**h1 a h6** - Definido para estruturar os titulos, ele sera dividido por grau de importancia de 1 para 6, sendo 1 mais importante. Isto nao tem haver com estilo (tamanho e cor é estilo)

**br** - quebra linha

**hr** - quebra linha horizontal

**<!-- -->** - Para fazer comentario, mas usado so para dividir codigo, pois ele aparece na inspecao

**a** - Tag para adicionar link e posterior inserir uma descricao.
- **target** - serve para indicar a abertura do link em uma nova aba, devemos usar 'target="_blank"'

**assets ou img** - convencao para depositar as imagens a serem usadas no html, sempre criar uma pasta na raiz onde esta o index.

**img** - para indicar uma imagem.
- **alt** - toda tag img deve ter um attr chamado 'alt', ele serve para descrever a img para a internet, assim é possivel pesquisar o que tem na pagina.

**Listas** - podem ser ordenas pela tag **ol** ou nao ordenadas pela tag **ul**. Dentro delas deve entrar a tag **li**.

**Tabelas** - Nao devem ser utilizadas, mas caso precise:
- **table** - para criar a tabela
- **tr** - fica a linha
- **td** - fica os dados
- **th** - fica o cabecalho

**div** - para criar divisao no site, para encapsular elementos do site.

**figure** - para definir area de uma img.
**figcaption** - para descrever para o buscador o que temos na img.

**blockquote** - para definir citações.

**form** - para abrir formulario.
**input** - temos tipos de input diferentes para definir o proposito.
- *Tipo text* - para receber texto.
- *submit* - se refere a um btn para enviar dados.
- *textarea* - é uma area maior para digitar texto grandes.
- *fieldset* - utilizado para vincular varios input em uma area somente.
- *password* - para utilizacao de senha, escondendo o que esta sendo digitado.
- *reset* - para limpar o formulario, ele é um btn.
- *radio* - para selecionar uma de várias opcoes que estao amostra.
- *checkbox* - ao contrario da radio, este posso marcar mais de uma opcao.
- *date* - insercao de data. 
- *file* - para enviar arquivos.
- *number* - para input de numeros com auxilio da seta.
- *email* - é um input especial para validacao do email.
**atributos** - o form possui os seguintes attr:
- *action* - envio de dados.
- *name* - este valor é pego quando o attr é enviado.
- *for* - serve para dar nome da label e boa pratica é colocar o mesmo nome do
 input.
- *value* - serve para deixar um valor ja preenchido.
- *disabled* - serve para bloquear o input quando nao queremos que seja feito.
- *placeholder* - para adicinar dicas dentro dos input.
- *required* - para forçar o usuario a inserir o valor no input, se ele nao fizer, sera levantado um aviso.
**method** - o form possui os seguintes metodos:
- *get ou post* - receber ou enviar dados.
**select** - para definir opcoes (lista).
- *selected* - é uma attr do select para pre definir uma das opcoes da lista.
- *multiple* - para selecionar multiplas selecoes.
- *datalist* - é uma opção de lista que mostra para o usuario as opcoes a serem selecionadas ou pre digitadas. 

## SEPARAÇÃO ESTRUTURAL DENTRO DO HTML
**Tags de separação do html para melhor semântica da estrutura do arquivo:**
- *nav* - para colocar tudo que é de navegação do site, em relação ao menu.
- *main* - onde fica a parte de conteúdo principal.
- *section* - subdivisão dentro do html para definir que ali eu tenho "div" de conteúdo específico.
- *aside* - para colocar informacoes laterais no site, este conteudo nao sera varrido pelo google.
- *figure e figcaption* - a primeira tag é a pai e a segunda é a filha, para descrição da imagem para busca do google.
- *mark* - para dar evidência a uma parte do texto.



---

# CSS

Dentro do html sempre direcionamos a pagina de estilos no head da pagina pelo cmd '<link rel="stylesheet" href="css/styles.css">'.

## ORDEM DO CSS
- Se tiver tudo junto, o CSS ira dar preferencia para esta sequencia: inline, interno e externo.
- *classe e Id*, são elementos mais especificos. Id nao pode se repetir, mas as classes sim.
- *cores*, não é indicado usar nomes nas cores. O ideal é usar RGB ou Hexa que é o mais usado. No Hexa o 0 é a mais escura e F a mais clara, a cada duas casa é a definicao de verm, verde, azul.
**#000** é preto e **#FFF** é branco.
- Separar o seletor por "," faz com que ele aproveite configuracoes. 

## TAGS do CSS:

**Uso de Variaveis no CSS** - podemos criar variaveis para nao ficar repetindo cores ou errar o nome:
    *Construcao variavel:*
        ':root {
            --bg: #fff;
            --texto: #111;
            --acao: #2563eb;
        }'

    *Uso da variavel:*
        body {
            background-color: var(--bg);
            counter-reset: var(--texto);
        }


**padding** - cria um espaço dentro da margem e dentro do border.

**back-ground-color** - cor de fundo.

- *box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);* - Esta config faz com que caixas "div", fiquem com um leve sobreado em volta dando um visual de flutuar.

**background** - cor de fundo através de funcao.
- *.login-btn:hover {background: linear-gradient(90deg, #8a2be2, #6a5acd);}* - funcao para tornar um btn com degrade de cores. Usar um hover alternando a posicao das cores para dar um efeito.

**opacity** - ele esta para o back_color, ele joga uma opacidade, que vai de 0 a 1.

**.nome_classe** - o "." e nome significa a tag para classe do elemento. Ex. no html '''<p class="parag"> Teste de texto com classe</p>'''. 

**#nome_id** - modo de especificar o css do ID. Ex: '<p class="parag" id="importante"> Teste de texto sem classe</p>'

**font-size** - tamano da fonte.

**color** - Cor da letra.

**border** - para borda.
**border-radius** - arredonda a borda.

**background-image** - para colocar imagem no background. Importante, eu insiro a img pelo css. EX: 'background-image: url("../img/nature.jpg")'
**background-position** - para centralizar a img dentro do elemento "div", neste caso colocamos com valor *center*.
**background-size** - para centralizar a img dentro do elemento "div", neste caso colocamos com valor *cover*. **Os dois juntos centraliza e reduz a imagem dentro da div**

**height e width** - se diz a respeito do tamanho da div.
- *height: 100vh* - usa a altura de tela para definir o tamanho da div.

**overflow-x: hidden** - serve para pegar uma div e extender ela até o final da ocupação em x (na horizontal).

**box-sizing** - Serve para redimensionar o espaco interno do conteudo com o tamanho maximo determinado pelo width. Se o w=500, mesmo que minha imagem tenho 500 e meu padding 50, o css transformara o a imagem em 400 para colocar dois padding de 50. Cmd: *box-sizing=boder-box*

**text-align** - alinhamento de texto dentro do container.

**text-decoration** - coloca o underline, line-through e none para colocar linha, riscado ou nada em qq texto.

**text-transform** - para transformar o texto em cx alta e baixa.

**line-height** - define uma altura de ocupacao do texto dentro de um container, usamos o mesmo valor que o height para centralizar o texto.

**letter-spacing** - espaçamento entre letras.

**cursor** - possui as opçoes:
- *pointer* - quando ficar em cima do elemento o cursor muda para uma maozinha.

**font-family** - determinar a familia de possiveis fontes.
**font-style** - definicao do tipo oblico e negrito.
**font-weight** - define a espessura da fonte. Sendo o normal para este attr é 300.
**font-size** - determina o tam da fonte.
**list-style: none** - remove marcacoes no LI de uma lista.

**flex** - define o como o elemento irá aumentar se ocorrer um zoom na página. Seu params: 1 1 200px (os dois primeiros é para ratio durante o zoom e o último é o tamanho dos elementos).

**display** - muda o comportamento de bloco ou inline para os containers do html. 
- *Inline-block* - joga uma do lado da outra.
- *None* - esconde o container.
- *flex* - deixa as div um do lado do outro. Usado para acondicionar os containers.
    - *justify-content: space-between* - espalha em espaco iguais as divs que estao lado a lado para ocupar a tela.
    - *flex-warp* - usado para display flex, ao colocar esta tag na div pai (.warp), ele passa a respeitar minhas div filhas ao qual o with é 33% da tela. Neste caso ela criara 3 espaços dentro de .box e coloca mais 3 espacos abaixo e assim por diante. Ex:
    '.warp {
    display: flex;
    margin-bottom: 20px;
    flex-wrap: wrap;
    }

    .box {
        height: 40px;
        width: 33%;
        border: 1px solid red;
    }'
    - *flex-direction* - define uma direcao para div:
        - *flex-direction: column* - joga as div em uma coluna.
    - *justify-content: end* - Joga as div para o final a direita da tela.
    - *justify-content: around* - Deixa espaços iguais em cada div que está dentro do container.
    - *align-items: center*  - Alinhamento no centro da div pai na vertical.
    - *align-items: stretch* - estica o elemento para cobrir toda a div pai na vertical.
    - *gap* - tag para gerar espacamento entre os elementos dentro de uma div que está regida pelo flex.
    - *order* - reposiciona o elemento dentro da div flex de acordo com sua posicao via id number.
    - *flex: 2* - é uma funcao que tonar a div que eu coloquei esta tag, como duas vezes o tamanho de suas div vizinhas do mesmo flex. Para lancar mais foco na div que contém isto.
    - *flex-basis: 20px* - Este caso trabalha junto com o flex:2, isto é, para as div filhas que tiverem com esta tag, elas terao 20px de largura e as demais que tivera com *flex-grow: 1*, elas aumentarao o tamanho até fechar a largura da tela., assim posso usar o *flex-shrink: 2*, ele irá diminuir o tamnho em 2x mais do que os outros elementos da mesma div flex.
    - *align-self: center* - tag para fazer a div específica esquecer a orientaçao das outras div e ela mesmo assumir sua propria posicao.

**position** - serve para posicionar os elementos na tela, sendo da esquerda para direita, do topo para parte inferior Lembrando que todo elemento é estatico e comeca com um padrao. Segue suas variantes:
- *static* - é posicao padrao, ela segue o fluxo do html
- *relative* - top, left, right e botton move o elemento pela tela, a partir da posicao que ele deveria iniciar se fosse static.
- *fixed* - defino uma posicao que ele sempre ficara na tela, mesmo que a tela mova, ele ficara visivel.
- *absolute* - top, eft, right e botton move o elemento pela tela, a partir da posicao do canto direito superior da tela.
- *absolute com relative* - top, left, right e botton move o elemento pela tela, a partir do elemento mais próximo dentro do container. Jogamos uma div dentro da outra para controlar cada uma de uma forma.
- *sticky* - top, left, right e botton move o elemento pela tela, mas o comportamento é ele assumir a posicao dele até que entre na tela de acordo com a sequencia de containers do html, apos entrar na tela, ele fica em uma posicao imposta no css, sendo assim, mesmo que mova a tela, ele sempre respeitara a posicao imposta, a nao ser que voltemos a tela para posicao original.
- *z-index* - serve para colocar elementos que estao sobrepostos, em uma posicao de hierarquia. Por ex. se o elem A precisa ficar sobre o elem B, o z-index de A sera =1 e de B sera =2.

**@media** - tag para assumir no css novos parametros de acordo com o tamanho de tela do browser. Sua sintaxe: 'screen and (max-width: 500px) { aqui vai o css }'.
Para esconder em landscape, a sintaxe é: *'screen and (orientation: landscape)'*

- *600px para baixo* - para trabalhar com celular
- *768px a 600px* - para tablets
- *992px a 768px* - mini laptops
- *992px para cima* - laptops e desktop 


