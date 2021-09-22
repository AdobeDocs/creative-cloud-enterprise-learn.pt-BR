---
title: Dicas e técnicas para dominar a iluminação 3D na CGI
description: Saiba mais sobre iluminação 3D e como criar diferentes condições de luz que podem alterar completamente uma cena gerada por computador e a aparência dos objetos nela
role: User
level: Beginner, Intermediate
keywords: Iluminação 3D, 600 MSV global
exl-id: 05eb729e-35b8-46e2-9c56-590250097d0b
source-git-commit: e3982cf31ebb0dac5927baa1352447b3222785c9
workflow-type: tm+mt
source-wordcount: '2738'
ht-degree: 0%

---

# Dicas e técnicas para dominar a iluminação 3D na CGI

Saiba mais sobre a iluminação 3D e como criar diferentes condições de luz que podem alterar completamente uma cena gerada por computador e a aparência dos objetos nela.

Percebemos o mundo à nossa volta usando os nossos sentidos. ouvimos, sentimos, cheiramos, vemos. Podemos ver porque nossos olhos estão captando informação trazida a nós por partículas elementares chamadas fótons. Esta informação é processada pelo nosso cérebro para produzir uma imagem. O que interpretamos como uma cor de objeto, brilho, translucidez ou qualidades metálicas são todos produtos da interação entre os fótons e a superfície do objeto.

A mecânica da luz em uma cena 3D gerada por computador segue o mesmo princípio natural de dispersão de fótons, através de um processo chamado [traçado de raios](https://en.wikipedia.org/wiki/Ray_tracing_(graphics)). Os raios saltam das formas e interagem com seus materiais, definindo efetivamente como os objetos aparecem na imagem final. As luzes expõem a dimensionalidade de qualquer coisa que existe em uma cena 3D.

Alguns materiais são mais sensíveis às condições de iluminação do que outros. Tome metais, por exemplo: um objeto cromático reflete basicamente tudo ao seu redor. Se uma luz for movida, se tornar mais clara ou maior, todas essas informações serão visíveis diretamente na superfície do cromo em detalhes quase semelhantes aos do espelho, de modo que podem parecer completamente diferentes de uma condição de luz para outra.

![Uma cena CGI 3D de um carro em um estacionamento com um sinal de neon na parede. A iluminação muda de luz do dia para LED neon emanando do sinal](assets/Mastering3dlighting_1.gif)

## Como trabalhar com luzes 3D para criar renderizações 3D eficazes

O processo de criação de uma renderização 3D nunca é o mesmo, mas estes são os passos mais comuns:

1. Criação ou aquisição de objetos
1. Montagem da cena
1. Enquadramento da cena
1. **Iluminação**
1. Criação ou atribuição de material
1. Renderização

Quando você chega à fase de iluminação, é ideal configurar as luzes antes de trabalhar nos materiais. Para fazer isso, você pode atribuir um material cinza neutro fosco à cena inteira. Dessa forma, você poderá ver e entender mais claramente como as luzes afetam as silhuetas do objeto na cena. Após a conclusão dos materiais, a iluminação pode precisar de mais refinamento.

![A sala de estar CGI renderiza a comparação com o material cinza neutro à esquerda em comparação com os materiais acabados à direita](assets/Mastering3dlighting_2.jpg)

É melhor trabalhar nas luzes, uma de cada vez. A luz ativa deve ser a única visível na cena, enquanto todas as outras luzes devem ser desativadas temporariamente. Dessa forma, você poderá ver como uma luz específica influencia a cena e alterar isso trabalhando em suas propriedades, como posição, direção, intensidade etc.

![Exemplo de 3 luzes que iluminam individualmente um modelo de carro 3D e todas as três que trabalham em conjunto](assets/Mastering3dlighting_3.gif)

Outro truque útil é criar uma esfera com um material metálico brilhante (um cromo ou espelho). Essa &quot;esfera espelhada&quot; refletirá efetivamente a cena inteira ao redor, para que você possa determinar facilmente a posição, a direção ou o tamanho da luz. No caso das luzes ambiente, você poderá ver seu reflexo na esfera espelhada, o que ajudará a configurar sua orientação no espaço.

![Usar uma esfera de espelho (esfera com textura metálica) para ver e orientar a luz ambiente em uma cena 3D](assets/Mastering3dlighting_4.gif)

## Tipos de luzes em Adobe [!DNL Dimension]

### Luzes ambientais

As luzes ambiente são imagens equirretangulares (esféricas), que são envolvidas em toda a cena. Como o nome sugere, essas luzes servem para emular todo o ambiente, inclusive as fontes de luz, que estão armazenadas nelas.

![Exemplos de luzes ambiente feitas de fotos, uma cena de estúdio 3D e uma cena 3D abstrata](assets/Mastering3dlighting_5.jpg)

Quando você cria uma nova cena em [[!DNL Dimension]](https://www.adobe.com/products/dimension.html), uma luz de ambiente padrão será criada para você. É por isso que você consegue imediatamente ver qualquer coisa na cena. Adobe [!DNL Dimension] Ativos iniciais incluem um certo número de luzes de ambiente, que podem ser experimentadas imediatamente. Além disso, [Adobe [!DNL Stock]](https://stock.adobe.com/search?filters[content_type:3d]=1&amp;filter[3d_type_id][0]=2&amp;load_type=3d+lp) oferece uma enorme seleção com curadoria de luzes ambiente.

As luzes do ambiente produzem resultados altamente realistas e podem poupar muito tempo. Para conseguir algo semelhante manualmente, você teria que criar todo o ambiente em 3D (incluindo várias fontes de luz), o que é uma quantidade significativa de trabalho.

![Exemplo de uma cena em que todo o conjunto (incluindo as luzes) foi montado em 3D para obter resultados semelhantes aos de estúdio](assets/Mastering3dlighting_6.jpg)

Há muitas maneiras de criar luzes ambiente, incluindo capturar de uma cena 3D, de uma fotografia, e usar sistemas paramétricos. Se a luz ambiente for feita de uma cena 3D, o processo é simples. A imagem de saída precisa ser de 32 bits, o que capturará as informações de luz de todas as luzes na cena. A câmera 3D precisa usar a projeção equirretangular (para produzir uma imagem esférica).

![Exemplo de uma cena iluminada por uma luz ambiente de estúdio 3D](assets/Mastering3dlighting_7.jpg)

![Uma luz ambiente de estúdio 3D é criada pela renderização de uma cena 3D de um estúdio em uma imagem equirretangular de 32 bits](assets/Mastering3dlighting_8.png)

Você também pode criar luzes ambiente capturando fotografias do mundo real. Para esse fluxo de trabalho, uma câmera 360 é necessária (por exemplo, [Ricoh Theta Z1](https://theta360.com/en/about/theta/z1.html)). A câmera é então usada para bracketing de exposição, ou para tirar várias fotos do mesmo ambiente, tiradas com um intervalo de diferentes valores de exposição (de subexposição a superexposição). Essas capturas são então usadas para construir imagens de 32 bits, geralmente chamadas de HDRs (curto para um intervalo dinâmico alto). Uma maneira de montar tal imagem é com a função Mesclar para HDR no Photoshop. O intervalo de exposição incorporado se tornará a propriedade de intensidade.

![Exemplo de uma cena 3D iluminada por uma luz fotográfica Ambiente](assets/Mastering3dlighting_9.jpg)

![A luz do ambiente fotográfico é criada usando a combinação de exposição e Mesclar para HDR Pro no Photoshop](assets/Mastering3dlighting_10.jpg)

Em ambos os casos, as fontes de luz (e suas intensidades) são &quot;cozidas&quot; nessas imagens e emitirão a luz assim que forem usadas em [!DNL Dimension].

Nesses métodos, você capturou toda a iluminação, reflexos e detalhes necessários, mas os aplicativos 3D permitem que você continue editando-os no espaço 3D, para que você possa ajustar a rotação da iluminação, bem como alterar a intensidade e a cor geral.

![Manipulação da intensidade e orientação de uma luz ambiente em uma cena 3D](assets/Mastering3dlighting_11.gif)

### Luzes direcionais

Além das luzes Ambiente, que emitem luz de 360 graus, há também luzes direcionais, que emitem luz apenas de uma direção. Eles são usados para emular lanternas e outros tipos de luzes provenientes de um emissor bem definido, e podem ser moldados como um círculo ou um quadrado.

O uso de luzes direcionais oferece controle total sobre a configuração de iluminação. Iluminar a cena usando essas luzes é feito da mesma forma que na fotografia tradicional, onde cada luz pode ser controlada de maneira independente, permitindo que você crie sua própria iluminação fotográfica virtual. Uma das configurações de iluminação mais usadas é o sistema de luz de 3 pontos.

[!DNL Dimension] tem uma ação conveniente, Aim leve no ponto, que permite controlar a rotação e a altura simplesmente clicando e arrastando através de um objeto 3D. Dessa forma, você pode direcionar dinamicamente os raios de luz. Esses parâmetros também podem ser ajustados manualmente.

Você pode alterar a cor e a intensidade das luzes direcionais, bem como ajustar a forma da fonte de luz - fazê-la circular ou retangular, esticá-la ou deixá-la maior. Finalmente, é possível suavizar as bordas da fonte de luz.

![Modificar a forma de uma luz direcional no Adobe  [!DNL Dimension]](assets/Mastering3dlighting_12.gif)

Se você tornar a fonte de luz menor que o objeto, as sombras serão mais nítidas, com um contorno mais nítido, porque os raios não podem ultrapassar o objeto iluminado. Fontes de luz maiores produzem sombras mais suaves, porque nesse caso os raios vêm de todos os lados do objeto (marcados em vermelho na ilustração abaixo), criando uma matriz de sombras. Essas sombras são suavizadas pelos raios que vêm da direção oposta.

![Diagrama que ilustra o efeito que a intensidade, a direção e o tamanho da iluminação têm no modo como um objeto 3D é iluminado e na sombra que ele projeta](assets/Mastering3dlighting_13.jpg)

![Exemplo de como o tamanho de uma luz 3D afeta a suavidade da sombra projetada por um modelo de carro CGI](assets/Mastering3dlighting_14.gif)

### Sol e céu

A luz do sol é um tipo especial de luz direcional. O processo de configuração é muito semelhante a uma luz direcional regular, mas essa luz altera automaticamente a cor com a altura; quando estiver próximo do horizonte (valores de ângulo de baixa altura), tornar-se-á gradualmente mais quente para simular o pôr do sol. A cor também pode ser alterada usando predefinições. Enquanto isso, a opacidade afetará a suavidade da sombra.

![Manipulação de propriedades de iluminação para iluminação solar em um modelo de carro 3D em Adobe  [!DNL Dimension]](assets/Mastering3dlighting_15.gif)

![Uma cena 3D na lua onde a única fonte de iluminação é a luz do sol](assets/Mastering3dlighting_16.jpg)

Somos capazes de emular o céu usando luzes ambiente, e qualquer luz ambiente que apresente o céu pode ser usada. Agora, temos que alinhar a luz solar (feita em [!DNL Dimension]) com o Sol, capturada na luz ambiente. Uma maneira rápida de fazer isso é criar uma esfera e atribuir um material metálico a ela. isto nos fornecerá reflexões em tempo real do ambiente, para que possamos usar a luz Aim no ponto para alinhar a luz solar com o Sol.

Se a luz do ambiente apresentar um céu coberto, a propriedade de opacidade pode ser usada para combinar mais estreitamente essas condições.

![Manipulação de propriedades de opacidade para iluminação do ambiente do céu em um modelo de carro 3D no Adobe  [!DNL Dimension]](assets/Mastering3dlighting_17.gif)

Depois que a luz do sol e a luz do ambiente do céu estiverem emparelhadas, você poderá girá-las juntas usando a propriedade Rotação global.

### Luzes baseadas em objeto

Os objetos podem ser transformados em fontes de luz, ativando a propriedade Brilho para seus materiais. Dessa forma, é possível criar objetos como lâmpadas, luzes de néon, softboxes e todos os tipos de telas e exibições.

O benefício-chave do uso desse tipo de iluminação é a queda de intensidade, que produz resultados muito naturais. Isso é bastante útil para visualização de produtos ou outras cenas com base em estúdio.

![Fonte de luz com declínio (uma chapa brilhante) VS uma fonte de luz infinita (uma luz direcional)](assets/Mastering3dlighting_18.png)

Você pode controlar a suavidade das sombras, escalando o objeto brilhante para cima ou para baixo, usando a ferramenta de transformação. Aumentar a intensidade da luz também aumenta.

![Alterar o tamanho da luz do objeto aumentará a intensidade da luz e suavizará as sombras](assets/Mastering3dlighting_19.gif)

Diferentemente dos tipos anteriores de luzes que cobrimos, essas luzes também podem utilizar texturas, além de cores simples. As texturas podem ser anexadas à cor base de seus materiais, e a intensidade da luz é controlada por meio de um controle deslizante de brilho.

![Aplicação de uma textura a uma luz de objeto iluminando um modelo de carro 3D](assets/Mastering3dlighting_20.gif)

## Exemplos de iluminação 3D eficaz

### Iluminação do produto

![Exemplo de 3 luzes (chave, preenchimento e jante) iluminando um modelo de fone de ouvido 3D individualmente e todas as três trabalhando juntas](assets/Mastering3dlighting_21.gif)

Há muitas técnicas fotográficas para configurar a luz para uma tomada de produto. Usaremos uma das configurações mais usadas, que é o sistema de luz de 3 pontos.

Essa configuração consiste em três luzes:

1. **Luz chave:** usada como fonte primária, isso brilha aproximadamente da direção da câmera

   ![Exemplo de luz de tecla iluminando um modelo de fone de ouvido 3d](assets/Mastering3dlighting_22.jpg)

1. **Luz da borda:** orientada no lado oposto da tecla, é usada para expor a silhueta do assunto.

   ![Exemplo de luz da jante iluminando um modelo de fone de ouvido 3D](assets/Mastering3dlighting_23.jpg)

1. **Luz de preenchimento:** menos intensivo e servindo para preencher áreas mais escuras, isso é usado para áreas que as duas luzes anteriores não atingem.

   ![Exemplo de luz de preenchimento iluminando um modelo de fone de ouvido 3d](assets/Mastering3dlighting_24.jpg)

Há duas maneiras de criar a iluminação de 3 pontos em [!DNL Dimension] - usando luzes direcionais (adicionando-as individualmente à cena ou usando uma predefinição de Luz de 3 pontos) ou por meio de objetos brilhantes.

![Exemplo de configuração de luz de 3 pontos em uma cena 3D](assets/Mastering3dlighting_25.jpg)

![Um softbox de uma configuração de iluminação 3D é desconstruído em um quadro, lâmpadas e tela](assets/Mastering3dlighting_26.jpg)

### Iluminação criativa

![Arte 3D entitulada por Pipe Dreams por Vladimir Petkovic](assets/Mastering3dlighting_27.jpg)

Iluminação criativa é usada onde a precisão física não é o objetivo principal. Isso inclui cenas abstratas e surreais de todos os tipos, então não há limites reais onde nossa imaginação possa nos levar.

No exemplo acima, a ideia era retratar um ambiente como sonho: cores doces, pastéis e superfícies lisas. O sistema de iluminação é feito de três placas brilhantes (duas na lateral e a principal na parte inferior). Todas as chapas brilhantes são irrealisticamente grandes, o que cria sombras e realces muito suaves. As fontes de luz são coloridas e essa cor é transferida para o material atribuído aos objetos na cena.

O objeto da cena (tubulações) está completamente cercado pela geometria das paredes. Isso fará com que os raios de luz saltem para frente e para trás e se misturem de maneiras interessantes. Brincar com tons quentes VS frios geralmente produz um bom contraste (esta técnica é usada às vezes em fotografias em retrato).

![Ilustração que demonstra a configuração de iluminação 3D para os sonhos de Pipe de Vladimir Petkovic](assets/Mastering3dlighting_28.jpg)

### Visualização interior

![Uma cena interior 3D de uma sala de estar](assets/Mastering3dlighting_29.jpg)

Criar uma visualização de um interior 3D segue um certo conjunto de regras, que quase sempre garante bons resultados. Para esse caso de uso, consideraremos apenas a luz natural (sem fontes artificiais, como lâmpadas).

Em primeiro lugar, uma cena como esta precisa estar num ambiente fechado. Assim como na vida real, o interior precisará de paredes, chão, teto e janelas. Isso garantirá que a luz atravesse as janelas e, em seguida, salte (por meio de um processo chamado rastreamento de raio). Esse comportamento produz iluminação muito natural (por exemplo, as áreas ocultadas, como cantos, serão mais escuras).

Como a cena está quase completamente cercada por geometria arquitetônica, veremos muito pouca iluminação e quase nenhum reflexo vindo da luz do ambiente. No entanto, neste caso, estamos realmente construindo nosso próprio ambiente, que é o próprio interior. Então a luz reagirá com os objetos na cena, saltando deles e as paredes ao redor. Os objetos refletirão apenas uns aos outros e as paredes ao seu redor. No entanto, é uma boa ideia acrescentar uma luz do ambiente, apresentando o céu. Isso adicionará algum preenchimento azul difuso.

A maneira mais fácil de definir essa luz é usando planos com materiais brilhantes. Nesse caso de uso temos três aviões, que cobrem todas as aberturas no interior.

![Uma ilustração que demonstra como as luzes chave e de preenchimento são posicionadas em uma sala de estar 3D para iluminar a cena](assets/Mastering3dlighting_30.jpg)

A intensidade da luz é controlada pela propriedade de brilho nos materiais dos aviões. Você pode adicionar uma cor ou mesmo uma textura, que pode ser usada para projetar sombras interessantes. O uso de materiais de brilho também propiciará a queda da intensidade da luz, o que é muito importante para a iluminação interior.

![Exemplo de luz ambiente, ambiente e luz-chave, e ambiente, luzes-chave e de preenchimento iluminando uma cena de sala de estar 3D](assets/Mastering3dlighting_31.gif)

### Iluminação exterior

![Cena de um toco de árvore no chão da floresta, interligada com fios e fitas CGI iluminadas com iluminação 3D ao ar livre](assets/Mastering3dlighting_32.jpg)

Criar iluminação ao ar livre é bastante simples e se resume ao uso de um sistema de luz solar e do céu (veja acima). É importante combinar a luz do sol corretamente com a luz do ambiente baseada no céu - prestando atenção tanto à orientação como ao valor de opacidade.

A cena em si tem um grande papel nisso. Para produzir resultados atraentes, use objetos em sua cena como catalisadores que interagem com a luz. Na renderização da floresta mostrada acima, os objetos (várias plantas, toras e árvores) são colocados próximos uns dos outros.

![Objetos em uma cena de floresta 3D indicam como a luz interage com o ambiente](assets/Mastering3dlighting_33.png)

Isso significa que haverá muita interação complexa de traçado de raios, à medida que a luz sopra entre os objetos. As manchas sombreadas aparecerão escuras (como esperado), enquanto as áreas expostas permanecerão claras.

![Usando a Rotação Global no Adobe  [!DNL Dimension] para reorientar o sistema de luz do Sol e do Céu em uma cena 3D](assets/Mastering3dlighting_34.gif)

Espero que esta visão geral ilustre a importância de dominar as luzes 3D em várias situações. Você deve estar pronto para começar a produzir resultados mais atraentes.

Boa iluminação! Baixe a [versão mais recente](https://creativecloud.adobe.com/apps/download/[!DNL Dimension]) do Dimension hoje mesmo.
