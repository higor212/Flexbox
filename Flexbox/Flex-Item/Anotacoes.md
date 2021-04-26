# Flex Itens
Os flex itens são filhos diretos do Flex Container.
É possível que um Flex Item seja também um Flex Container ao definir um **display: flex;** ao mesmo.

# Flex Grow

Define a habilidade de um flex item crescer.Por padrão o valor é 0, assim os flex itens ocupam um tamanho máximo relacionado ao conteúdo interno deles ou ao width definido.  

Ao definir o valor 1 para todos os flex itens, eles vão tentar ter a mesma largura e vão ocupar 100% do container.
Caso um elemento possua um conteúdo muito largo ele irá respeitar o mesmo.

Caso houver uma linha com quatro itens, onde três deles são flex-grow: 1 e um flex-grow: 2, o flex-grow: 2 tentará ocupar 2 vezes mais espaço extra do que os outros elementos.

**OBS:** O justify-content não irá funcionar em itens com flex-grow definido.

# Flex Basis

Indica o tamanho inicial do flex item antes da distribuição de espaço restante.

## flex-basis: auto;

É o padrão da propriedade, ele faz com que a largura da base seja igual a do item. Caso o item não tiver o tamanho especificado, o tamanho será de acordo com o conteúdo.
Vale lembrar que o valor padrão da propriedade é 0 como padrão assim como o flex-grow.

## flex-basis: unidade;

Pode ser rem, em, px, %, e etc

## flex-basis: 0;

O flex-basis ( flex: 1) faz com que todos os itens tenham tamanhos iguais independentemente do conteúdo dentro dos itens.

## flex-basis: número;

Irá atribuir a largura dos itens de acordo com o valor que for colocado.
Ele diminui de acordo com o container também.

# Flex Shrink

Define a capacidade de redução de tamanho do item.

## flex-shrink: 1;

Valor padrão, permite que os itens tenham os seus tamanhos reduzidos para caber no container. Sendo o tamanho definido por width ou por flex-basis.

# Flex

Atalho para as propriedades, flex-grow, flex,shrink e flex-basis.
O melhor a ser feito para consistência entre os navegadores, utilizar essa propriedade do que todas as propriedaes separadas.

## flex: 0 1 auto;

Valor padrão, sempre vai ser 0 de flex-grow, 1 de flex-shrink e auto de basis.

## flex: 1;

Flex-grow e flex-shrink será 1 e o flex-basis 0, alguns browsers esse valor vai ser 0%.

# Order

Modifica a ordem dos itens do container, do menor para maior.

# Align Self

Serve para definir o alinhamento de um **item especifíco** dentro do container.

## align-self: auto;
Valor inicial padrão. Vai respeitar o que for definido pelo align-items no flex-container.

## align-self: flex-start;
Alinha o item ao início.

## align-self: flex-end;
Alinha o item ao final.

## align-self: center;
Alinha o item ao centro.

## align-self: baseline;
Alinha o item a linha de base.

## align-self: stretch;
Estica o item.







