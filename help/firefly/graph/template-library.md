---
title: Biblioteca de modelos
description: Procure por modelos de Firefly prontos para abrir e adaptar ao seu próprio projeto
feature: Image Editing, Gen AI
role: User
level: Beginner
jira: KT-
hide: true
hidefromtoc: true
source-git-commit: 1b6b9793b2fa33365ccf6fb0f049632a67f09cae
workflow-type: tm+mt
source-wordcount: '390'
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

Retorne ao [Introdução ao Firefly Graph](https://experienceleague.adobe.com/pt-br/docs/creative-cloud-enterprise-learn/cce-learning-hub/fireflyoverview/firefly-graph/overview-firefly-graph).