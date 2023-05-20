---
title: Dicas e técnicas para dominar a iluminação 3D em CGI
description: Saiba mais sobre a iluminação 3D e como criar diferentes condições de luz que podem alterar completamente uma cena gerada por computador e a aparência dos objetos
role: User
level: Beginner, Intermediate
keywords: Iluminação 3D, 600 Global MSV
exl-id: 05eb729e-35b8-46e2-9c56-590250097d0b
source-git-commit: 01d80f9b296bc7d13b5e931cf0ca22d1335271dc
workflow-type: tm+mt
source-wordcount: '2739'
ht-degree: 0%

---

# Dicas e técnicas para dominar a iluminação 3D em CGI

Saiba mais sobre a iluminação 3D e como criar diferentes condições de luz que podem alterar completamente uma cena gerada por computador e a aparência dos objetos.

Percebemos o mundo à nossa volta usando nossos sentidos: ouvimos, sentimos, cheiramos, vemos. Podemos ver porque nossos olhos estão captando informações trazidas a nós por partículas elementares chamadas fótons. Esta informação é processada pelo nosso cérebro para produzir uma imagem. O que interpretamos como uma cor de objeto, brilho, translucidez ou qualidades metálicas são produtos da interação entre os fótons e a superfície do objeto.

Mecânicos de luz em uma cena 3D gerada por computador seguem o mesmo princípio natural de dispersão de fótons, através de um processo chamado [traçado de raio](https://en.wikipedia.org/wiki/Ray_tracing_(graphics)). Os raios saltam das formas e interagem com seus materiais, definindo efetivamente como os objetos aparecem na imagem final. As luzes expõem a dimensionalidade de tudo o que existe em uma cena 3D.

Alguns materiais são mais sensíveis às condições de iluminação do que outros. Tomemos como exemplo os metais: um objeto cromado basicamente reflete tudo ao seu redor. Se uma luz é movida, fica mais clara, ou maior, toda essa informação é visível diretamente na superfície do cromo em detalhes quase como espelhos, de modo que pode parecer completamente diferente de uma condição de luz para a outra.

![Uma cena CGI 3D de um carro em um estacionamento com uma placa de néon na parede. A iluminação muda da luz do dia para um LED néon que emana do sinal](assets/Mastering3dlighting_1.gif)

## Como trabalhar com luzes 3D para criar renderizações 3D eficazes

O processo de criar uma renderização 3D nunca é totalmente o mesmo, mas estas são as etapas mais comuns:

1. Criação ou aquisição de objeto
1. Montagem da cena
1. Enquadrar a cena
1. **Iluminação**
1. Criação ou atribuição de material
1. Renderizando

Quando você chegar à fase de iluminação, é ideal para configurar suas luzes antes de trabalhar nos materiais. Para fazer isso, você pode atribuir um material cinza neutro e fosco à cena inteira. Dessa forma, você poderá ver e entender mais claramente como as luzes afetam as silhuetas dos objetos na cena. Após a conclusão dos materiais, a iluminação pode precisar de mais refinamento.

![Comparação de renderização de sala de estar CGI com material fosco cinza neutro à esquerda em comparação com materiais acabados à direita](assets/Mastering3dlighting_2.jpg)

É melhor trabalhar com as luzes uma de cada vez. A luz ativa deve ser a única visível na cena, enquanto todas as outras luzes devem estar temporariamente desligadas. Dessa forma, você poderá ver como uma luz específica influencia a cena e alterá-la trabalhando em suas propriedades, como posição, direção, intensidade etc.

![Exemplo de 3 luzes iluminando um modelo de carro 3d individualmente e todos os 3 deles trabalhando juntos](assets/Mastering3dlighting_3.gif)

Outro truque útil é criar uma esfera com um material metálico brilhante (um cromo ou um espelho). Essa &quot;bola espelhada&quot; refletirá efetivamente toda a cena ao redor, para que você possa determinar facilmente a posição, a direção ou o tamanho da luz. No caso das luzes ambiente, você poderá ver seu reflexo na bola espelho, o que ajudará a configurar sua orientação no espaço.

![Uso de uma esfera de espelho (com textura metálica) para ver e orientar a luz ambiente em uma cena 3D](assets/Mastering3dlighting_4.gif)

## Tipos de luzes em Adobe [!DNL Dimension]

### Luzes ambiente

As luzes ambiente são imagens equirretangulares (esféricas), que são colocadas ao redor de toda a cena. Como o nome sugere, essas luzes servem para emular todo o ambiente, incluindo as fontes de luz, que são armazenadas nelas.

![Exemplos de luzes de ambiente feitas de fotos, uma cena de estúdio 3D e uma cena 3D abstrata](assets/Mastering3dlighting_5.jpg)

Ao criar uma cena no [[!DNL Dimension]](https://www.adobe.com/products/dimension.html), uma luz ambiente padrão será criada para você. É por isso que você é imediatamente capaz de ver qualquer coisa na cena. Adobe [!DNL Dimension] Os ativos iniciais incluem um determinado número de luzes de ambiente, que você pode experimentar imediatamente. Além disso, [Adobe [!DNL Stock]](https://stock.adobe.com/search?filters[content_type:3d]=1&amp;filters[3d_type_id][0]=2&amp;load_type=3d+lp) oferece uma seleção enorme e com curadoria de luzes ambiente.

As luzes ambiente produzem resultados altamente realistas e podem poupar muito tempo. Para conseguir algo semelhante manualmente, você teria que criar todo o ambiente em 3D (incluindo várias fontes de luz), o que é uma quantidade significativa de trabalho.

![Exemplo de uma cena em que todo o conjunto (incluindo as luzes) foi montado em 3D para alcançar resultados semelhantes aos de um estúdio](assets/Mastering3dlighting_6.jpg)

Há muitas maneiras de criar luzes ambiente, incluindo capturar de uma cena 3D, de uma fotografia e usar sistemas paramétricos. Se a luz ambiente for criada a partir de uma cena 3D, o processo será simples. A imagem de saída precisa ser de 32 bits, o que capturará as informações de luz de todas as luzes na cena. A câmera 3D precisa usar a projeção equirretangular (para gerar uma imagem esférica).

![Exemplo de uma cena iluminada por um estúdio 3D Luz ambiente](assets/Mastering3dlighting_7.jpg)

![Uma luz ambiente de estúdio 3D é criada renderizando uma cena 3D de um estúdio em uma imagem equirretangular de 32 bits](assets/Mastering3dlighting_8.png)

Você também pode criar luzes ambiente capturando fotografias do mundo real. Para esse fluxo de trabalho, é necessária uma câmera 360 (por exemplo, [Ricoh Theta Z1](https://theta360.com/en/about/theta/z1.html)). A câmera é então usada para o suporte de exposição ou para tirar várias fotos do mesmo ambiente, tiradas com uma faixa de diferentes valores de exposição (de subexposta a superexposta). Essas capturas são então usadas para construir imagens de 32 bits, geralmente chamadas de HDRs (abreviação de High Dynamic Range). Uma maneira de montar essa imagem é com a função Mesclar para HDR no Photoshop. O intervalo de exposição incorporado se tornará a propriedade de intensidade.

![Exemplo de uma cena 3D iluminada por uma luz ambiente fotográfica](assets/Mastering3dlighting_9.jpg)

![A luz ambiente fotográfica é criada usando o suporte de exposição e Mesclar com HDR Pro no Photoshop](assets/Mastering3dlighting_10.jpg)

Em ambos os casos, as fontes de luz (e suas intensidades) são &quot;cozidas&quot; nessas imagens e emitirão a luz assim que forem usadas [!DNL Dimension].

Nesses métodos, você capturou toda a iluminação, os reflexos e os detalhes necessários, mas os aplicativos 3D permitem continuar editando-os no espaço 3D, para que você possa ajustar a rotação da iluminação, bem como alterar a intensidade e a cor gerais.

![Manipular a intensidade e a orientação de uma luz ambiente em uma cena 3D](assets/Mastering3dlighting_11.gif)

### Luzes direcionais

Além das luzes ambiente, que emitem luz a partir de 360 graus, há também luzes direcionais, que emitem luz a partir de uma única direção. Elas são usadas para emular lanternas e outros tipos de luzes vindas de um emissor bem definido, e elas podem ser moldadas como um círculo ou um quadrado.

Usar luzes direcionais oferece controle total sobre a configuração de iluminação. A iluminação da cena usando essas luzes é feita da mesma forma que na fotografia tradicional, onde cada luz pode ser controlada de maneira independente, permitindo que você crie sua própria iluminação fotográfica virtual. Uma das configurações de iluminação mais usadas é o sistema de luz de 3 pontos.

[!DNL Dimension] tem uma ação conveniente, Apontar luz no ponto, que permite controlar a rotação e a altura simplesmente clicando e arrastando sobre um objeto 3D. Dessa forma, você pode direcionar os raios de luz dinamicamente. Esses parâmetros também podem ser ajustados manualmente.

Você pode alterar a cor e a intensidade das luzes direcionais, bem como ajustar a forma da fonte de luz - torná-la circular ou retangular, esticá-la ou torná-la maior. Finalmente, você pode suavizar as bordas da fonte de luz.

![Modificação da forma de uma luz direcional em Adobe [!DNL Dimension]](assets/Mastering3dlighting_12.gif)

Se você tornar a fonte de luz menor que o objeto, as sombras ficarão mais nítidas, com um contorno mais nítido, porque os raios não podem passar pelo objeto iluminado. Fontes de luz maiores produzem sombras mais suaves, porque nesse caso os raios vêm de todos os lados do objeto (marcados em vermelho na ilustração abaixo), criando uma matriz de sombras. Essas sombras são suavizadas pelos raios vindos da direção oposta.

![Diagrama que ilustra o efeito que a intensidade, a direção e o tamanho da iluminação têm na maneira como um objeto 3D é iluminado e na sombra que ele projeta](assets/Mastering3dlighting_13.jpg)

![Exemplo de como o tamanho de uma luz 3D afeta a suavidade da sombra projetada por um modelo de carro CGI](assets/Mastering3dlighting_14.gif)

### Sol e céu

A luz solar é um tipo especial de luz direcional. O processo de configuração é muito semelhante a uma luz direcional regular, no entanto, esta luz mudará automaticamente a cor com a altura; quando estiver perto do horizonte (valores de ângulo de altura baixa), vai gradualmente se tornar mais quente para simular o pôr do sol. A cor também pode ser alterada usando predefinições. Enquanto isso, a nebulosidade afetará a suavidade da sombra.

![Manipulação de propriedades de iluminação para a luz do sol em um modelo de carro 3D em Adobe [!DNL Dimension]](assets/Mastering3dlighting_15.gif)

![Uma cena em 3D na lua onde a única fonte de iluminação é a luz do sol](assets/Mastering3dlighting_16.jpg)

Somos capazes de emular o céu usando luzes ambiente, e qualquer luz ambiente com o céu pode ser usada. Agora, temos que alinhar a luz do sol (feita em [!DNL Dimension]) com o Sol, captada na luz ambiente. Uma maneira rápida de fazer isso é criar uma esfera e atribuir um material metálico a ela; isso nos fornecerá reflexões do ambiente em tempo real, para que possamos usar a luz do Aim nesse ponto para alinhar a luz do sol com o sol.

Se a luz ambiente apresenta um céu nublado, a propriedade de nebulosidade pode ser usada para corresponder mais estreitamente a essas condições.

![Manipulação de propriedades de nebulosidade para a iluminação ambiente do céu em um modelo de carro 3D em Adobe [!DNL Dimension]](assets/Mastering3dlighting_17.gif)

Quando a luz do sol e a luz ambiente do céu estiverem emparelhadas, você poderá girá-las juntas usando a propriedade Rotação global.

### Luzes baseadas em objeto

Os objetos podem ser transformados em fontes de luz, ativando a propriedade Brilho para seus materiais. Dessa forma, é possível criar objetos como lâmpadas, luzes neon, softboxes e todos os tipos de telas e monitores.

O principal benefício do uso desse tipo de iluminação é a queda de intensidade, que produz resultados muito naturais. Isso é muito útil para visualização de produto ou outras cenas baseadas em estúdio.

![Fonte de luz que tem uma queda (uma placa brilhante) VS uma fonte de luz infinita (uma luz direcional)](assets/Mastering3dlighting_18.png)

Você pode controlar a suavidade das sombras dimensionando o objeto com brilho para cima ou para baixo usando a ferramenta de transformação. Torná-lo maior também aumentará a intensidade da luz.

![Alterar o tamanho da luz do objeto aumentará a quantidade de luz e suavizará as sombras](assets/Mastering3dlighting_19.gif)

Diferentemente dos tipos de luzes anteriores, essas luzes também podem usar texturas, além de cores simples. As texturas podem ser anexadas à cor de base de seus materiais, e a intensidade da luz é controlada por meio de um controle deslizante de brilho.

![Aplicar uma textura a um objeto iluminando um modelo de carro 3D](assets/Mastering3dlighting_20.gif)

## Exemplos de iluminação 3D eficaz

### Iluminação do produto

![Exemplo de 3 luzes (chave, preenchimento e aro) iluminando um modelo de fone de ouvido 3D individualmente e todos os 3 deles trabalhando juntos](assets/Mastering3dlighting_21.gif)

Há muitas técnicas fotográficas para configurar a luz de uma foto de produto. Usaremos uma das configurações mais usadas, que é o sistema de luz de 3 pontos.

Essa configuração consiste em três luzes:

1. **Luz principal:** usado como fonte principal, brilha aproximadamente a partir da direção da câmera

   ![Exemplo de uma luz principal iluminando um modelo de fone de ouvido 3d](assets/Mastering3dlighting_22.jpg)

1. **Luz da jante:** orientado no lado oposto da tecla, isso é usado para expor a silhueta do assunto.

   ![Exemplo de uma luz de aro iluminando um modelo de fone de ouvido 3d](assets/Mastering3dlighting_23.jpg)

1. **Luz de preenchimento:** menos intensiva e que serve para preencher áreas mais escuras, é usada para áreas que as duas luzes anteriores não alcançam.

   ![Exemplo de uma luz de preenchimento iluminando um modelo de fone de ouvido 3d](assets/Mastering3dlighting_24.jpg)

Há duas maneiras de criar a iluminação de 3 pontos no [!DNL Dimension] - usando luzes direcionais (adicionando-as individualmente à cena ou usando uma predefinição de Luz de 3 pontos) ou por meio de objetos brilhantes.

![Exemplo de uma configuração de luz de 3 pontos em uma cena 3D](assets/Mastering3dlighting_25.jpg)

![Um softbox de uma configuração de iluminação 3D é desconstruído em um quadro, lâmpadas e tela](assets/Mastering3dlighting_26.jpg)

### Iluminação criativa

![Ilustração 3D intitulada Pipe Dreams de Vladimir Petkovic](assets/Mastering3dlighting_27.jpg)

A iluminação criativa é usada onde a precisão física não é o objetivo principal. Isso inclui cenas abstratas e surreais de todos os tipos, então não há limites reais onde nossa imaginação possa nos levar.

No exemplo acima, a ideia era retratar um ambiente de sonho: doces, cores pastel e superfícies lisas. O sistema de iluminação é feito de três placas brilhantes (duas na lateral e a principal brilhando na parte inferior). Todas as placas brilhantes são irrealisticamente grandes, o que cria sombras e realces muito suaves. As fontes de luz são coloridas e essa cor é transferida para o material atribuído aos objetos na cena.

O objeto da cena (tubos) é completamente cercado pela geometria das paredes. Isso fará com que os raios de luz saltem para frente e para trás e se misturem de maneiras interessantes. Tocar com tons frios VS quentes geralmente produz um contraste agradável (essa técnica às vezes é usada em fotografia de retrato).

![Uma ilustração que demonstra a configuração de iluminação 3D para os sonhos de tubos de Vladimir Petkovic](assets/Mastering3dlighting_28.jpg)

### Visualização interior

![Uma cena interior 3D de uma sala de estar](assets/Mastering3dlighting_29.jpg)

Criar uma visualização de um interior 3D segue um determinado conjunto de regras, o que quase sempre garante bons resultados. Para este caso de uso, consideraremos apenas luz natural (sem fontes artificiais, como lâmpadas).

Em primeiro lugar, uma cena como essa precisa estar em um ambiente fechado. Assim como na vida real, o interior precisará de paredes, chão, teto e janelas. Isso garantirá que a luz atravesse as janelas e depois salte (por um processo chamado traçado de raio). Esse comportamento produz uma iluminação muito natural (por exemplo, as áreas obstruídas, como cantos, serão mais escuras).

Como a cena é quase completamente cercada pela geometria arquitetônica, veremos muito pouca iluminação e quase nenhuma reflexão vinda da luz Ambiente. No entanto, neste caso, estamos na verdade construindo nosso próprio ambiente, que é o próprio interior. Então a luz reagirá com os objetos na cena, saltando deles e das paredes ao redor. Os objetos refletirão apenas uns aos outros e as paredes ao redor deles. No entanto, é uma boa ideia adicionar uma luz ambiente, apresentando o céu. Isso adicionará um preenchimento azul difuso.

A maneira mais fácil de definir essa luz é usando planos com materiais brilhantes. Neste caso de uso temos três planos, que cobrem todas as aberturas no interior.

![Uma ilustração que demonstra como as luzes de tecla e preenchimento são posicionadas no interior de uma sala de estar 3D para iluminar a cena](assets/Mastering3dlighting_30.jpg)

A intensidade da luz é controlada pela propriedade de brilho nos materiais dos planos. Você pode adicionar uma cor ou até mesmo uma textura, que pode ser usada para projetar sombras interessantes. O uso de materiais de brilho também fornecerá a queda de intensidade da luz, que é muito importante para a iluminação interior.

![Exemplo de luz ambiente, ambiente e luz principal, e ambiente, luzes chave e preenchimento iluminando uma cena de sala de estar 3d](assets/Mastering3dlighting_31.gif)

### Iluminação exterior

![Uma cena de um toco de árvore em um chão de floresta, entrelaçada com fios e fitas CGI iluminados com iluminação 3D ao ar livre](assets/Mastering3dlighting_32.jpg)

Criar iluminação externa é bastante simples e se resume a usar um sistema de luz solar e do céu (veja acima). É importante combinar a luz do sol corretamente com a luz ambiente baseada no céu - prestando atenção tanto à orientação quanto ao valor de nebulosidade.

A cena em si tem um papel importante nisso. Para produzir resultados atraentes, use objetos na cena como catalisadores que interagem com a luz. Na renderização da floresta mostrada acima, os objetos (várias plantas, troncos e árvores) são colocados próximos uns dos outros.

![Objetos em uma cena de floresta 3D indicam como a luz interagirá com o ambiente](assets/Mastering3dlighting_33.png)

Isso significa que haverá muita interação complexa de traçado de raios, à medida que a luz salta entre os objetos. Os pontos sombreados aparecerão escuros (como esperado), enquanto as áreas expostas permanecerão brilhantes.

![Uso da rotação global no Adobe [!DNL Dimension] para reorientar o sistema de luz do Sol e do Céu em uma cena 3D](assets/Mastering3dlighting_34.gif)

Espero que esta visão geral ilustre a importância de dominar as luzes 3D em várias situações. Você deve estar pronto para começar a produzir resultados mais atraentes.

Boa iluminação! Baixe o [versão mais recente](https://creativecloud.adobe.com/apps/download/Dimension) de Dimension hoje.
