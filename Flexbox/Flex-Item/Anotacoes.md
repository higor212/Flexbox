# Flex Itens
Os flex itens são filhos diretos do Flex Container.
É possível que um Flex Item seja também um Flex Container ao definir um **display: flex;** ao mesmo.

# Flex Grow

Define a habilidade de um flex item crescer.Por padrão o valor é 0, assim os flex itens ocupam um tamanho máximo relacionado ao conteúdo interno deles ou ao width definido.  

Ao definir o valor 1 para todos os flex itens, eles vão tentar ter a mesma largura e vão ocupar 100% do container.
Caso um elemento possua um conteúdo muito largo ele irá respeitar o mesmo.

Caso houver uma linha com quatro itens, onde três deles são flex-grow: 1 e um flex-grow: 2, o flex-grow: 2 tentará ocupar 2 vezes mais espaço extra do que os outros elementos.

**OBS:** O justify-content não irá funcionar em itens com flex-grow definido.