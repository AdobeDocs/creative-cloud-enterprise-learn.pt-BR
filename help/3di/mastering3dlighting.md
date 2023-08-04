---
title: Dicas e técnicas para dominar a iluminação 3D na CGI
description: Saiba mais sobre iluminação 3D e como criar diferentes condições de luz que podem alterar completamente uma cena gerada por computador e a aparência dos objetos nela
feature: 3D
role: User
level: Beginner, Intermediate
keywords: Iluminação 3D, 600 Global MSV
exl-id: 05eb729e-35b8-46e2-9c56-590250097d0b
source-git-commit: e39efe0f7afc4e3e970ea7f2df57b51bf17123a6
workflow-type: tm+mt
source-wordcount: '2733'
ht-degree: 0%

---

# Dicas e técnicas para dominar a iluminação 3D na CGI

Saiba mais sobre iluminação 3D e como criar diferentes condições de luz que podem alterar completamente uma cena gerada por computador e a aparência dos objetos nela.

Percebemos o mundo ao nosso redor usando nossos sentidos: ouvimos, sentimos, cheiramos e vemos. Podemos ver porque nossos olhos estão captando a informação trazida a nós por partículas elementares chamadas fótons. Esta informação é processada pelo nosso cérebro para produzir uma imagem. O que interpretamos como uma cor de objeto, brilho, translucidez ou qualidades metálicas são todos produtos da interação entre os fótons e a superfície do objeto.

A mecânica da luz em uma cena 3D gerada por computador segue o mesmo princípio natural de dispersão de fótons, usando um processo chamado traçado de raio (ray tracing). Os raios colidem com as formas e interagem com seus materiais, definindo efetivamente como os objetos aparecem na imagem final. As luzes expõem a dimensionalidade de qualquer coisa que existe em uma cena 3D.

Alguns materiais são mais sensíveis às condições de iluminação do que outros. Vamos usar o metal como exemplo, um objeto cromático reflete basicamente tudo ao seu redor. Se uma luz for movida, se tornar mais clara ou maior, todas essas informações serão visíveis diretamente na superfície cromada em detalhes quase semelhantes aos de um espelho, portanto, ela pode parecer completamente diferente de uma condição de luz para a outra.

![Uma cena CGI 3D de um carro em um estacionamento com uma placa de neon na parede. A iluminação passa de luz do dia para um LED de néon que emana do letreiro](assets/Mastering3dlighting_1.gif)

## Como trabalhar com luzes 3D para criar renderizações eficazes

O processo de criação de uma renderização 3D nunca é o mesmo, mas estes são os passos mais comuns:

1. Criação ou aquisição de objetos
1. Montagem da cena
1. Enquadrar a cena
1. **Iluminação**
1. Criação ou atribuição de material
1. Renderizando

Quando você chega à fase de iluminação, é ideal configurar as luzes antes de trabalhar nos materiais. Para fazer isso, você pode atribuir um material cinza neutro fosco à cena inteira. Dessa forma, você poderá ver e entender mais claramente como as luzes afetam as silhuetas do objeto na cena. Depois que os materiais forem concluídos, a iluminação pode precisar de mais refinamento.

![Comparação da sala de estar CGI com material fosco cinza neutro à esquerda com materiais acabados à direita](assets/Mastering3dlighting_2.jpg)

É melhor trabalhar nas luzes, uma de cada vez. A luz ativa deve ser a única visível na cena, enquanto todas as outras luzes devem ser desativadas temporariamente. Dessa forma, você poderá ver como uma luz específica influencia a cena e pode alterá-la trabalhando em suas propriedades, como posição, direção, intensidade etc.

![Exemplo de três luzes que iluminam individualmente um modelo de carro 3D e todas as três que trabalham juntas](assets/Mastering3dlighting_3.gif)

Outro truque útil é criar uma esfera com um material metálico brilhante (um cromo ou um espelho). Essa “esfera espelhada” refletirá efetivamente a cena inteira ao redor, e você determinar facilmente a posição, a direção ou o tamanho da luz. No caso das luzes ambiente, você poderá ver seu reflexo na esfera espelhada, o que ajudará a configurar sua orientação no espaço.

![Usar uma esfera espelhada (esfera com textura metálica) para ver e orientar a luz ambiente em uma cena 3D](assets/Mastering3dlighting_4.gif)

## Tipos de luzes no Adobe [!DNL Dimension]

### Luzes ambiente

As luzes ambiente são imagens equirretangulares (esféricas), que são envolvidas por toda a cena. Como o nome sugere, essas luzes servem para emular todo o ambiente, inclusive as fontes de luz, que estão armazenadas nelas.

![Exemplos de luzes ambiente feitas de fotos, uma cena de estúdio 3D e uma cena 3D abstrata](assets/Mastering3dlighting_5.jpg)

Ao criar uma nova cena no [[!DNL Dimension]](https://www.adobe.com/products/dimension.html), uma luz de ambiente padrão será criada para você. É por isso que você consegue imediatamente ver qualquer coisa na cena. Adobe [!DNL Dimension] Os ativos iniciais incluem um certo número de luzes ambiente, que você pode experimentar imediatamente. Além disso, [Adobe [!DNL Stock]](https://stock.adobe.com/search?filters[content_type:3d]=1&amp;filters[3d_type_id][0]=2&amp;load_type=3d+lp) O oferece uma enorme seleção com curadoria de luzes ambiente.

As luzes do ambiente produzem resultados altamente realistas e podem poupar muito tempo. Para conseguir algo semelhante manualmente, você teria que criar todo o ambiente em 3D (incluindo várias fontes de luz), o que representa uma quantidade significativa de trabalho.

![Exemplo de uma cena em que todo o conjunto (incluindo as luzes) foi montado em 3D para obter resultados semelhantes aos de estúdio](assets/Mastering3dlighting_6.jpg)

Há muitas maneiras de criar luzes ambiente, incluindo capturar de uma cena 3D, de uma fotografia, e usar sistemas paramétricos. Se a luz ambiente for feita de uma cena 3D, o processo é simples. A imagem de saída precisa estar em 32 bits, o que capturará as informações de luz de todas as luzes na cena. A câmera 3D precisa usar a projeção equirretangular (para produzir uma imagem esférica).

![Exemplo de uma cena iluminada por uma Luz ambiente de estúdio 3D](assets/Mastering3dlighting_7.jpg)

![Uma luz ambiente de estúdio 3D é criada pela renderização de uma cena 3D de um estúdio em uma imagem equirretangular de 32 bits](assets/Mastering3dlighting_8.png)

Você também pode criar luzes ambiente capturando fotografias do mundo real. Para esse fluxo de trabalho, uma câmera 360 é necessária (por exemplo, [Ricoh Theta Z1](https://theta360.com/en/about/theta/z1.html)). A câmera é então usada para agrupar a exposição, ou para tirar várias fotos do mesmo ambiente, com intervalos de diferentes valores de exposição (de subexposição a superexposição). Essas capturas são então usadas para construir imagens de 32 bits, geralmente chamadas de HDRs (sigla para High Dynamic Range, Amplo Intervalo Dinâmico). Uma maneira de montar essa imagem é com a função Mesclar para HDR no Photoshop. O intervalo de exposição incorporado se tornará a propriedade de intensidade.

![Exemplo de uma cena 3D iluminada por uma Luz de Ambiente fotográfica](assets/Mastering3dlighting_9.jpg)

![A luz do ambiente fotográfico é criada usando o agrupamento de exposição e Mesclagem para HDR Pro no Photoshop](assets/Mastering3dlighting_10.jpg)

Em ambos os casos, as fontes de luz (e suas intensidades) são “cozidas” nessas imagens e emitirão a luz quando forem usadas [!DNL Dimension].

Nesses métodos, você capturou toda a iluminação, reflexos e detalhes necessários, mas os aplicativos 3D permitem que você continue editando-os no espaço 3D, para ajustar a rotação da iluminação e alterar a intensidade e a cor geral.

![Manipulação da intensidade e orientação de uma luz ambiente em uma cena 3D](assets/Mastering3dlighting_11.gif)

### Luzes direcionais

Além das Luzes ambiente, que emitem luz em 360 graus, existem também as luzes direcionais, que emitem luz em apenas de uma direção. Eles são usados para emular lanternas e outros tipos de luzes que partem de um emissor bem definido, e podem ter o formato de um círculo ou quadrado.

O uso de luzes direcionais oferece controle total sobre a configuração de iluminação. Iluminar a cena usando essas luzes funciona da mesma forma que na fotografia tradicional, em que cada luz pode ser controlada de forma independente, permitindo que você crie sua própria iluminação fotográfica virtual. Uma das configurações de iluminação mais usadas é o sistema de luz de três pontos.

[!DNL Dimension] tem uma ação conveniente, Mire a luz no ponto, que permite controlar a rotação e a altura simplesmente clicando e arrastando em um objeto 3D. Dessa forma, você pode direcionar dinamicamente os raios de luz. Esses parâmetros também podem ser ajustados manualmente.

Você pode alterar a cor e a intensidade das luzes direcionais e ajustar a forma da fonte de luz, dar uma forma circular ou retangular, esticá-la ou deixá-la maior. Finalmente, é possível suavizar as bordas da fonte de luz.

![Modificar a forma de uma luz direcional no Adobe [!DNL Dimension]](assets/Mastering3dlighting_12.gif)

Se você tornar a fonte de luz menor que o objeto, as sombras e os contornos serão mais nítidos, porque os raios não podem ultrapassar o objeto iluminado. Fontes de luz maiores produzem sombras mais suaves, porque nesse caso os raios chegam de todos os lados do objeto (marcados em vermelho na ilustração abaixo), criando uma matriz de sombras. Essas sombras são suavizadas pelos raios que vêm da direção oposta.

![Diagrama que ilustra o efeito que a intensidade, a direção e o tamanho da iluminação têm no modo como um objeto 3D é iluminado e na sombra que ele projeta](assets/Mastering3dlighting_13.jpg)

![Exemplo de como o tamanho de uma luz 3D afeta a suavidade da sombra projetada por um modelo de carro CGI](assets/Mastering3dlighting_14.gif)

### Sol e céu

A luz do sol é um tipo especial de luz direcional. O processo de configuração é muito semelhante ao de uma luz direcional regular, mas essa luz altera automaticamente a cor com a altura; quando estiver próximo do horizonte (valores de ângulo de baixa altura), se tornará gradualmente mais quente para simular o pôr do sol. A cor também pode ser alterada usando predefinições. Enquanto isso, a opacidade afetará a suavidade da sombra.

![Manipulação de propriedades de iluminação para iluminação solar em um modelo de carro 3D em Adobe [!DNL Dimension]](assets/Mastering3dlighting_15.gif)

![Uma cena 3D na lua onde a única fonte de iluminação é a luz do sol](assets/Mastering3dlighting_16.jpg)

Somos capazes de emular o céu usando luzes ambiente, e qualquer luz ambiente que apresente o céu pode ser usada. Agora, temos que alinhar a luz do sol (feita em [!DNL Dimension]) com o Sol, capturada na luz ambiente. Uma maneira rápida de fazer isso é criar uma esfera e atribuir um material metálico a ela. Isto nos dará imagens refletidas em tempo real do ambiente, para que possamos Mirar a luz no ponto para alinhar a luz solar com o Sol.

Se a luz do ambiente apresentar um céu coberto, a propriedade de opacidade pode ser usada para combinar mais fielmente essas condições.

![Manipulação de propriedades de opacidade para iluminação do ambiente do céu em um modelo de carro 3D no Adobe [!DNL Dimension]](assets/Mastering3dlighting_17.gif)

Depois que a luz do sol e a luz do ambiente do céu estiverem emparelhadas, você pode girá-las juntas usando a propriedade Rotação global.

### Luzes baseadas em objeto

Os objetos podem ser transformados em fontes de luz, ativando a propriedade Brilho dos seus materiais. Dessa forma, é possível criar objetos como lâmpadas, luzes de néon, softboxes e todos os tipos de telas e exibições.

O principal benefício do uso desse tipo de iluminação é a queda de intensidade, que produz resultados muito naturais. Isso é muito útil para visualização de produtos ou outras cenas com estúdio.

![Fonte de luz com declínio (uma superfície brilhante) vs. uma fonte de luz infinita (uma luz direcional)](assets/Mastering3dlighting_18.png)

Você pode controlar a suavidade das sombras, ao ajustar o objeto brilhante para cima ou para baixo, usando a ferramenta de transformação. Tornar o objeto maior também aumentará a intensidade da luz.

![Alterar o tamanho da luz do objeto aumentará a intensidade da luz e suavizará as sombras](assets/Mastering3dlighting_19.gif)

Diferentemente dos tipos anteriores de luzes que abordamos, essas luzes também podem utilizar texturas, além de cores simples. As texturas podem ser anexadas à cor de base de seus materiais, e a intensidade da luz é controlada por meio de um controle deslizante de brilho.

![Aplicação de uma textura a uma luz de objeto iluminando um modelo de carro 3D](assets/Mastering3dlighting_20.gif)

## Exemplos de iluminação 3D eficaz

### Iluminação do produto

![Exemplo de três luzes (principal, preenchimento e recorte) iluminando um modelo de fone de ouvido 3D individualmente e todas as três trabalhando juntas](assets/Mastering3dlighting_21.gif)

Há muitas técnicas fotográficas para configurar a luz em uma foto de produto. Usaremos uma das configurações mais usadas, que é o sistema de luz de três pontos.

Essa configuração consiste em três luzes:

1. **Luz da tecla:** usado como a fonte principal, brilha aproximadamente na direção da câmera

   ![Exemplo de luz principal iluminando um modelo de fone de ouvido 3D](assets/Mastering3dlighting_22.jpg)

1. **Luz de recorte:** orientado no lado oposto da tecla, é usado para marcar a silhueta do assunto.

   ![Exemplo de luz de recorte iluminando um modelo de fone de ouvido 3D](assets/Mastering3dlighting_23.jpg)

1. **Luz de preenchimento:** menos intensa e atuando para preencher áreas mais escuras, usada para áreas que as duas outras luzes não atingem.

   ![Exemplo de uma luz de preenchimento iluminando um modelo de fone de ouvido 3D](assets/Mastering3dlighting_24.jpg)

Há duas maneiras de criar a iluminação de três pontos no [!DNL Dimension] - usando luzes direcionais (adicionando-as individualmente à cena ou usando uma predefinição de Luz de 3 pontos) ou por meio de objetos brilhantes.

![Exemplo de configuração de luz de três pontos em uma cena 3D](assets/Mastering3dlighting_25.jpg)

![Um softbox de uma configuração de iluminação 3D é representado por um quadro, luzes e tela](assets/Mastering3dlighting_26.jpg)

### Iluminação criativa

![Ilustração 3D intitulada Pipe Dreams de Vladimir Petkovic](assets/Mastering3dlighting_27.jpg)

A iluminação criativa é usada onde a precisão física não é o objetivo principal. Isso inclui cenas abstratas e surreais de todos os tipos, dessa forma, não há limites reais em que nossas imaginações possam nos levar.

No exemplo acima, a ideia era retratar um ambiente como sonho: cores doces, pastéis e superfícies lisas. O sistema de iluminação é feito de três painéis brilhantes (dois na lateral e o principal na parte inferior). Todas as placas brilhantes são desproporcionalmente grandes, o que cria sombras e realces muito suaves. As fontes de luz são coloridas e essa cor é transferida para o material atribuído aos objetos na cena.

O objeto da cena (a tubulação) está completamente cercado pela geometria das paredes. Isso faz com que os raios de luz saltem para frente e para trás e se misturem de maneiras interessantes. Brincar com tons quentes e frios geralmente produz um bom contraste (essa técnica é usada às vezes em fotografias de retrato).

![Uma ilustração que demonstra a configuração de iluminação 3D de Pipe Dreams de Vladimir Petkovic](assets/Mastering3dlighting_28.jpg)

### Visualização de interior

![Uma cena de interior 3D de uma sala de estar](assets/Mastering3dlighting_29.jpg)

Criar uma visualização de um interior 3D segue um certo conjunto de regras, que quase sempre garante bons resultados. Neste caso de uso, consideraremos apenas a luz natural (sem fontes artificiais, como lâmpadas).

Em primeiro lugar, uma cena como esta precisa estar num ambiente fechado. Assim como na vida real, o interior precisará de paredes, chão, teto e janelas. Isso garantirá que a luz passe pelas janelas e, em seguida, salte ao redor (por um processo chamado traçado de raio). Esse comportamento produz uma iluminação muito natural (por exemplo, as áreas ocultadas, como cantos, serão mais escuras).

Como a cena está quase que completamente cercada pela geometria da arquitetura, veremos muito pouca iluminação e quase nenhum reflexo vindo da luz do ambiente. No entanto, neste caso, estamos realmente construindo nosso próprio ambiente, que é o interior. Então a luz reagirá com os objetos na cena, sendo refletida por eles e pelas paredes ao redor. Os objetos refletirão apenas uns aos outros e as paredes ao seu redor. No entanto, é uma boa ideia acrescentar uma luz ao ambiente, caracterizando o céu. Isso adicionará um pouco de preenchimento azul difuso.

A maneira mais fácil de definir essa luz é usando planos com materiais brilhantes. Neste caso de uso temos três aviões, que cobrem todas as aberturas no interior.

![Uma ilustração que demonstra como as luzes principal e de preenchimento são posicionadas em uma sala de estar 3D para iluminar a cena](assets/Mastering3dlighting_30.jpg)

A intensidade da luz é controlada pela propriedade de brilho nos materiais dos aviões. Você pode adicionar uma cor ou até mesmo uma textura, que pode ser usada para projetar sombras interessantes. O uso de materiais brilhantes também diminui a intensidade da luz, o que é muito importante para a iluminação interior.

![Exemplo de luz ambiente, luz ambiente e principal e luzes ambiente, principal e de preenchimento iluminando uma cena de sala de estar 3D](assets/Mastering3dlighting_31.gif)

### Iluminação exterior

![Uma cena de um toco de árvore no chão da floresta, interligado com fios e fitas CGI iluminadas com iluminação 3D ao ar livre](assets/Mastering3dlighting_32.jpg)

Criar iluminação ao ar livre é bastante simples e se resume ao uso de um sistema de luz solar e do céu (veja acima). É importante combinar a luz do sol corretamente com a luz do ambiente baseada no céu, prestando atenção tanto à orientação quanto ao valor da opacidade.

A cena em si tem um grande papel nisso. Para produzir resultados atraentes, use objetos em sua cena como catalisadores que interagem com a luz. Na renderização da floresta mostrada acima, os objetos (várias plantas, troncos e árvores) são colocados próximos uns dos outros.

![Os objetos em uma cena de floresta 3D indicam como a luz interage com o ambiente](assets/Mastering3dlighting_33.png)

Isso significa que haverá muita interação complexa de traçado de raios, à medida que a luz é refletida entre os objetos. Os pontos sombreados aparecerão escuros (como esperado), enquanto as áreas expostas permanecerão claras.

![Como usar a Rotação global no Adobe [!DNL Dimension] para reorientar o sistema de luz do Sol e do Céu em uma cena 3D](assets/Mastering3dlighting_34.gif)

Espero que esta visão geral mostre a importância de dominar as luzes 3D em várias situações. Você deve estar pronto para começar a produzir resultados mais atraentes.

Boa iluminação! Baixe o [versão mais recente](https://creativecloud.adobe.com/apps/download/Dimension) de Dimension hoje.
