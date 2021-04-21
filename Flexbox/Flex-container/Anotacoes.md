# Display Flex

## display: flex;

Torna o elemento um flex container automaticamente transformando todos os seus filhos diretos em flex itens.

Com o display flex, todos os itens do container irão ir para lado a lado
 1 2 3 4 
 diferentemente do display block que são um em baixo do outro e que ocupam 100% do display.

## flex-wrap

 Quando os itens não cabem dentro do container, será quebrado para outras linhas.

## flex-item

 Ao adicionar o flex: 1 os itens irão crescer com o objetivo de ocupar o tamanho total do container.

# Flex Direction

 O objetivo é definir a direção dos flex itens. Por padrão o flexbox é **em linha (row)**, a mudança de row para **columns(colunas)** acontece quando se precisa implementar a responsividade em um site mobile, ou seja, irão ser quebrados em coluna.

## flex-direction: row ;
Os itens irão ser exibidos em  linha. **( a b c )**

## flex-direction: row-reverse;
Os itens ainda serão exibidos em linha, porém irão ser virados ao contrário **( c b a )**

## flex-direction: column;
Os itens são exibidos em colunas. 

- a
- b
- c

## flex-direction: column-reverse;
Os itens são exibidos em colunas reversas.

- c
- b
- a

# Flex Wrap 

## flex-wrap: nowrap;
É o valor padrão, ele não irá quebrar as linhas

## flex-wrap: wrap;
Quebra a linha quando um dos itens não conseguir compactar o container

## flex-wrap: wrap-reverse;
Assim como o direction, irá acontecer o mesmo, os itens irão ser ao contrário, ou seja, a quebra de linha será na direção contrária

# Flex Flow 

É um atalho para as propriedades flex direction e flex wrap, porém não é muito utilizada por no geral quando alteramos o flex direction para column mantemos o nowrap.
Quando é utilizado ao contrário, é usado o flex direction para row e o wrap para wrap.

## flex-flow: row nowrap;
Conteúdo em linha e não quebra a linha

## flex-flow: row wrap;
Conteúdo em linha e quebra a linha

## flex-flow: column nowrap;
Conteúdo em em colunas e não quebra linhas

# Justify content

Responsável por alinhar os itens flex no container de acordo com a direção em que eles estão.
Essa propriedade só irá funcionar caso os itens não ocupem todo o container, caso for definido por exemplo flex: 1, a propriedade não irá mais funcionar.

## justify-content: flex-start;
Alinha os itens no inicio do flex.

## justify-content: flex-end;
Alinha os itens no final do flex.

## justify-content: flex-center;
Alinha os itens no centro

## justify-content: flex-space-between;
os ítens são distribuídos de forma igual ao longo da linha; o primeiro ítem junto à borda inicial da linha, o último junto à borda final da linha.

## justify-content: flex-space-around;
os ítens são distribuídos na linha com o mesmo espaçamento entre eles. 

## justify-content: flex-space-evenly;
Os itens são distribuídos de forma que o espaçamento entre dois itens ( e o espaçamento das bordas) seja igual.

# Align Items
O align-items alinha os itens de acordo com o eixo do container, o alinhamento será diferente quando o flex direction for row ou column.

## align-items: stretch;
Vai fazer com que os itens do container tenham o mesmo height de forma que preencham todo o container.

## align-items: flex-start;
Alinha todos os itens do flex container ao inicio do mesmo. ( diferenciado caso o flex-direction esteja como row ou column)

## align-items: flex-end;
Alinha todos os itens do flex container ao fim do mesmo. ( diferenciado caso o flex-direction esteja como row ou column)

## align-items: center;
Os itens do flex container alinhados ao centro

## align-items: baseline;
Alinha os itens do flex container como uma linha de base, mesmo diferente o tamanho dos itens a linha de base da tipografia será o mesmo.

## align-items: center & justify-content: center;
Alinhar o item do container no centro verticalmente ou horizontalmente.

# Align Content

Alinha as linhas do container de acordo com o eixo vertical.
Só irá funcionar caso houver mais de uma linha de flex-itens.
Para isso o flex-wrap precisa ser wrap. Caso não for definido um height para o container, a propriedade não irá influenciar no layout.

## align-content: stretch
Por padrão o align-content mantém essa propriedade, ele cresce juntamente com os conteúdos e quebra para a outra linha.

## align-content: flex-start;
Alinha todos os itens ao inicio do container, de forma que não estiquem os conteúdos, a linha dos itens irá ocupar o tamanho do item que for o maior da linha.

## align-content: flex-end;
Alinha todos os itens ao final do container, de forma que não estiquem os conteúdos, a linha dos itens irá ocupar o tamanho do item que for o maior da linha.

## align-content: space-between;
Alinha as linhas criando um espaçamento igual aos itens

## align-content: space-around;
Alinha as linhas criando um espaçamento igual aos itens, porém ele cria um espaçamento no inicio e no final e o espaço entre os itens.

