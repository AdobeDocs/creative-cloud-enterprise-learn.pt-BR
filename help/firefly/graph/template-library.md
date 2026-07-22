---
title: Biblioteca de modelos
description: Procure por modelos de Firefly prontos para abrir e adaptar ao seu próprio projeto
feature: Image Editing, Gen AI
role: User
level: Beginner
jira: KT-
hide: true
hidefromtoc: true
source-git-commit: af06d76d4cad7ccf7adeb845d71525480b68ea4f
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 0%

---

# &#x200B;5. Biblioteca de modelos

Um índice de referência rápida de modelos de Firefly, organizado pelo que cada um produz ou faz. Cada exemplo é um ponto de partida — troque sua própria marca, produto e prompts antes de usar um modelo na produção.

## Geração e estilo da imagem

* [**Introdução - Gerar uma imagem**](/help/firefly/graph/templates/get-started-gen-image.md) — Este modelo é um gráfico básico: um nó de prompt em um nó de geração em uma saída. Use-o como o primeiro modelo para abrir com qualquer novo usuário.
* [**Geração consistente de caracteres**](/help/firefly/graph/templates/character-gen.md) — Neste modelo de gráfico, você carrega uma imagem de referência de um caractere e, em seguida, troca a cena ou o prompt de pose para cada nova tomada. A referência de caractere permanece bloqueada enquanto a cena ao redor é alterada.
* [**Extração de estilo**](/help/firefly/graph/templates/style-extraction.md) — neste modelo de gráfico, você alimenta uma imagem de referência para extrair seu tratamento de cor, luz e textura. Em seguida, é possível aplicar esse tratamento a qualquer nova imagem executada no mesmo gráfico.
* [**Vibrações do pôr do sol**](/help/firefly/graph/templates/sunset-vibes.md) — neste modelo de gráfico, você pode criar uma imagem tipográfica 3D usando um prompt de texto. O modelo manipula o posicionamento e o equilíbrio de cores automaticamente.

## Segmentação e composição

* [**Introdução - Segmente uma imagem**](/help/firefly/graph/templates/get-started-segment-image.md) — Neste modelo de gráfico, você carrega qualquer imagem de origem e executa o nó de segmentação para isolar o assunto de seu plano de fundo. Combine um nó de substituição de plano de fundo para obter um recorte limpo.
* [**Compor e mesclar camadas**](/help/firefly/graph/templates/composite-blend-layers.md) — neste modelo de gráfico, você empilha um recorte de produto e uma cena de fundo como entradas de camada separadas. Ajuste o modo de mesclagem e os nós de iluminação até que a composição seja lida como uma tomada.
* [**Correção de cores seletivas**](/help/firefly/graph/templates/selective-color-correction.md) — neste modelo de gráfico, você mascara uma região específica que precisa de correção e define a cor de destino somente nesse nó. O restante da imagem passa pelo gráfico intocado.

## Vídeo e animação

* [**Introdução - Geração de vídeo**](/help/firefly/graph/templates/get-started-video-gen.md) — Neste modelo de gráfico, você alimenta uma arte estática aprovada e um prompt de animação curto. O modelo gera um corte de vídeo criado a partir dessa mesma arte principal em vez de uma nova tomada.
* [**Tempo de marcador VFX**](/help/firefly/graph/templates/bullet-time-vfx.md) — Neste modelo de gráfico, você alimenta um produto ou imagem de assunto herói para gerar uma sequência giratória de ângulos ao redor dele e, em seguida, costura a varredura de quadro congelado automaticamente.

## Storyboarding

* [**Texto para storyboard**](/help/firefly/graph/templates/text-to-storyboard.md) — neste modelo de gráfico, você substitui nós de entrada de texto por elementos da sua história. Cada linha se torna seu próprio quadro de storyboard, gerado em sequência e disposto para revisão como um único conjunto de painéis.
* [**Construtor de storyboards**](/help/firefly/graph/templates/storyboard-builder.md) — Neste modelo de gráfico, você constrói um storyboard cena por cena, adicionando um nó por batida da narrativa. Reordene os nós para testar uma sequência diferente antes de bloquear a ordem final dos painéis.

## 3D e caractere

* [**Sombreadores em tempo real**](/help/firefly/graph/templates/real-time-shaders.md) — neste modelo de gráfico, você começa com uma imagem e aplica três sombreadores personalizados diferentes e visualiza o resultado em tempo real. Ajuste os parâmetros de sombreador diretamente no nó em vez de renderizar do zero.
* [**Geração de modelo de caractere**](/help/firefly/graph/templates/character-model-generation.md) — neste modelo de gráfico, você cria um estilo animado 3D de uma ilustração. O modelo gera uma passagem de modelo 3D base pronta para ser entregue a um modelador para limpeza, em vez de iniciar a partir de uma cena em branco.
* [**Design de brinquedo de vinil**](/help/firefly/graph/templates/vinyl-toy-design.md) — neste modelo de gráfico, você insere uma referência de personagem ou mascote e a renderiza em uma forma de brinquedo de vinil estilizada. Há ângulos de rotação para uma plataforma de licenciamento ou revisão de produtos.
* [**Virar do Sketch para 3D**](/help/firefly/graph/templates/sketch-to-3d.md) — Neste modelo de gráfico, você transforma um esboço em um caractere 3D. O gráfico cria um giro 3D giratório a partir dele, pronto para uma revisão interna de design antes de qualquer protótipo físico.

## Modelos de produtos e marcas

* [**Visualização de marca**](/help/firefly/graph/templates/branding-visualization.md) — neste modelo de gráfico, saiba como visualizar o logotipo ou a marca em cenas de produtos. Alimentar as diretrizes de marca ou um logotipo e uma paleta de cores e o gráfico produz arte-chave estática e um movimento curto em uma execução, para que ambos os formatos permaneçam visualmente alinhados.
* [**Modelo de produto da marca**](/help/firefly/graph/templates/brand-product-mockup.md) — Neste modelo de gráfico, saiba como visualizar seu produto em diferentes cenas. Você solta uma renderização de produto ou foto no nó do modelo e o gráfico a coloca dentro de uma cena totalmente da marca, com iluminação e sombra correspondentes a essa cena automaticamente.
* [**Foto editorial**](/help/firefly/graph/templates/editorial-photoshoot.md) — neste modelo de gráfico, você carrega uma referência de modelo e troca a entrada de vestuário para cada novo visual. Os nós de pose e iluminação permanecem bloqueados no conjunto para proporcionar uma sensação editorial consistente.
* [**Estúdio fotográfico**](/help/firefly/graph/templates/photography-studio.md) — neste modelo de gráfico, você coloca uma renderização do produto no plano de fundo do estúdio e ajusta a iluminação até que o resultado pareça uma captura de estúdio real.
* [**Aplicar decalque às superfícies**](/help/firefly/graph/templates/decal-to-surfaces.md) — neste modelo de gráfico, você carrega o modelo do produto base e o ativo de decalque ou logotipo como entradas separadas. O modelo quebra o decalque na geometria da superfície para que siga os contornos corretamente.

## Operações de lote e consistência

* [**Gerador de sistema de design**](/help/firefly/graph/templates/design-system-generator.md) — neste modelo de gráfico, você gera um sistema de design com base em uma captura de tela do site. O gráfico produz um conjunto correspondente de ícones, padrões e componentes de layout em uma única execução em lote.
* [**Geração de headshots**](/help/firefly/graph/templates/headshots-generation.md) — Neste modelo de gráfico você harmoniza um lote de headshots corporativos. Carregue as fotos de origem, uma por pessoa, e o gráfico normalizará a iluminação, o plano de fundo e o corte em todo o conjunto em uma execução.

Retorne ao [Introdução ao Firefly Graph](https://experienceleague.adobe.com/en/docs/creative-cloud-enterprise-learn/cce-learning-hub/fireflyoverview/firefly-graph/overview-firefly-graph).