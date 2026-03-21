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

**padding** - cria um espaço dentro da margem e dentro do border.

**back-ground-color** - cor de fundo.
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

**box-sizing** - Serve para redimensionar o espaco interno do conteudo com o tamanho maximo determinado pelo width. Se o w=500, mesmo que minha imagem tenho 500 e meu padding 50, o css transformara o a imagem em 400 para colocar dois padding de 50. Cmd: *box-sizing=boder-box*

**text-align** - alinhamento de texto dentro do container.

**text-decoration** - coloca o underline, line-through e none para colocar linha, riscado ou nada em qq texto.

**text-transform** - para transformar o texto em cx alta e baixa.

**letter-spacing** - espaçamento entre letras.

**font-family** - determinar a familia de possiveis fontes.
**font-style** - definicao do tipo oblico e negrito.
**font-weight** - define a espessura da fonte. Sendo o normal para este attr é 300.
**font-size** - determina o tam da fontve.

**display** - muda o comportamento de bloco ou inline para os containers do html. 
- *Inline-block* - joga uma do lado da outra.
- *None* - esconde o container.

**position** - serve para posicionar os elementos na tela, sendo da esquerda para direita, do topo para parte inferior Lembrando que todo elemento é estatico e comeca com um padrao. Segue suas variantes:
- *static* - é posicao padrao, ela segue o fluxo do html
- *relative* - top, left, right e botton move o elemento pela tela, a partir da posicao que ele deveria iniciar se fosse static.
- *fixed* - defino uma posicao que ele sempre ficara na tela, mesmo que a tela mova, ele ficara visivel.
- *absolute* - top, eft, right e botton move o elemento pela tela, a partir da posicao do canto direito superior da tela.
- *absolute com relative* - top, left, right e botton move o elemento pela tela, a partir do elemento mais próximo dentro do container. Jogamos uma div dentro da outra para controlar cada uma de uma forma.
- *sticky* - top, left, right e botton move o elemento pela tela, mas o comportamento é ele assumir a posicao dele até que entre na tela de acordo com a sequencia de containers do html, apos entrar na tela, ele fica em uma posicao imposta no css, sendo assim, mesmo que mova a tela, ele sempre respeitara a posicao imposta, a nao ser que voltemos a tela para posicao original.
- *z-index* - serve para colocar elementos que estao sobrepostos, em uma posicao de hierarquia. Por ex. se o elem A precisa ficar sobre o elem B, o z-index de A sera =1 e de B sera =2.



