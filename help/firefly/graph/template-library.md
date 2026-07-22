---
title: Biblioteca de modelos
description: Procure por modelos de Firefly prontos para abrir e adaptar ao seu próprio projeto
feature: Image Editing, Gen AI
role: User
level: Beginner
jira: KT-
hide: true
hidefromtoc: true
source-git-commit: 5a555416c5f45ca92de7df48e4b7cf8418102269
workflow-type: tm+mt
source-wordcount: '610'
ht-degree: 0%

---

# &#x200B;5. Biblioteca de modelos

Um índice de referência rápida de modelos de Firefly, organizado pelo que cada um produz ou faz. Cada exemplo é um ponto de partida — troque sua própria marca, produto e prompts antes de usar um modelo na produção.

## Geração e estilo da imagem

* [**Introdução - Gerar uma imagem**](/help/firefly/graph/templates/get-started-gen-image.md) — Este modelo é um gráfico básico: um nó de prompt em um nó de geração em uma saída. Use-o como o primeiro modelo para abrir com qualquer novo usuário.
* [**Geração consistente de caracteres**](/help/firefly/graph/templates/character-gen.md) — no modelo de gráfico, você carrega uma imagem de referência de um caractere e, em seguida, troca a cena ou o prompt de pose para cada nova tomada. A referência de caractere permanece bloqueada enquanto a cena ao redor é alterada.
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

Retorne ao [Introdução ao Firefly Graph](https://experienceleague.adobe.com/pt-br/docs/creative-cloud-enterprise-learn/cce-learning-hub/fireflyoverview/firefly-graph/overview-firefly-graph).