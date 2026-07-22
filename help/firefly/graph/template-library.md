---
title: Biblioteca de modelos
description: Procure por modelos de Firefly prontos para abrir e adaptar ao seu próprio projeto
feature: Image Editing, Gen AI
role: User
level: Beginner
jira: KT-
hide: true
hidefromtoc: true
source-git-commit: aa0ae4747f081c69d8a01d3f9acdd7844cca6afe
workflow-type: tm+mt
source-wordcount: '996'
ht-degree: 2%

---

# &#x200B;5. Biblioteca de modelos

Um índice de referência rápida de modelos de Firefly, organizado pelo que cada um produz ou faz. Cada exemplo é um ponto de partida — troque sua própria marca, produto e prompts antes de usar um modelo na produção.

## Geração e estilo da imagem

| Modelo de gráfico | Descrição | [!BADGE Casos de uso]{type=Informative tooltip="Casos de uso"} |
|---|---|---|
| [**Introdução - Gerar uma imagem**](/help/firefly/graph/templates/get-started-gen-image.md) | Este modelo é um gráfico básico: um nó de prompt em um nó de geração em uma saída. Use-o como o primeiro modelo para abrir com qualquer novo usuário. | Varejo, Saúde, Educação |
| [**Geração consistente de caracteres**](/help/firefly/graph/templates/character-gen.md) | Neste modelo de gráfico, você carrega uma imagem de referência de um personagem e, em seguida, troca a cena ou o prompt de pose para cada nova tomada. A referência de caractere permanece bloqueada enquanto a cena ao redor é alterada. | Viagens, varejo, instituições de ensino |
| [**Extração de estilo**](/help/firefly/graph/templates/style-extraction.md) | Neste modelo de gráfico, você é alimentado em uma imagem de referência para extrair sua cor, luz e tratamento de textura. Em seguida, é possível aplicar esse tratamento a qualquer nova imagem executada no mesmo gráfico. | Viagens, varejo, bebidas |
| [**Vibrações do pôr do sol**](/help/firefly/graph/templates/sunset-vibes.md) | Neste modelo de gráfico, você pode criar uma imagem tipográfica 3D usando um prompt de texto. O modelo manipula o posicionamento e o equilíbrio de cores automaticamente. | Viagens, bebidas, varejo |

## Segmentação e composição

| Modelo de gráfico | Descrição | [!BADGE Casos de uso]{type=Informative tooltip="Casos de uso"} |
|---|---|---|
| [**Introdução - Segmente uma imagem**](/help/firefly/graph/templates/get-started-segment-image.md) | Neste modelo de gráfico, você carrega qualquer imagem de origem e executa o nó de segmentação para isolar o assunto de seu plano de fundo. Combine um nó de substituição de plano de fundo para obter um recorte limpo. | Saúde, Varejo, Automotivo |
| [**Compor e mesclar camadas**](/help/firefly/graph/templates/composite-blend-layers.md) | Neste modelo de gráfico, você empilha um recorte de produto e uma cena de plano de fundo como entradas de camada separadas. Ajuste o modo de mesclagem e os nós de iluminação até que a composição seja lida como uma tomada. | Bebidas, Varejo, Viagem |
| [**Correção de cores seletivas**](/help/firefly/graph/templates/selective-color-correction.md) | Neste modelo de gráfico, você mascara uma região específica que precisa de correção e define a cor de destino apenas nesse nó. O restante da imagem passa pelo gráfico intocado. | Comunicações e telecomunicações, varejo, finanças |

## Vídeo e animação

| Modelo de gráfico | Descrição | [!BADGE Casos de uso]{type=Informative tooltip="Casos de uso"} |
|---|---|---|
| [**Introdução - Geração de vídeo**](/help/firefly/graph/templates/get-started-video-gen.md) | Neste modelo de gráfico, você alimenta uma arte estática aprovada e um prompt de animação curto. O modelo gera um corte de vídeo criado a partir dessa mesma arte principal em vez de uma nova tomada. | Finanças, bebidas, varejo |
| [**VFX**](/help/firefly/graph/templates/bullet-time-vfx.md) de Marcador | Neste modelo de gráfico, você alimenta um produto ou imagem de objeto principal para gerar uma sequência giratória de ângulos ao redor dela e, em seguida, costura a varredura de quadro congelado automaticamente. | Atividades ao ar livre, varejo, automotivo |

## Storyboarding

| Modelo de gráfico | Descrição | [!BADGE Casos de uso]{type=Informative tooltip="Casos de uso"} |
|---|---|---|
| [**Texto para storyboard**](/help/firefly/graph/templates/text-to-storyboard.md) | Neste modelo de gráfico, você substitui nós de entrada de texto por elementos da matéria. Cada linha se torna seu próprio quadro de storyboard, gerado em sequência e disposto para revisão como um único conjunto de painéis. | Finanças, Varejo, Tecnologia |
| [**Construtor de storyboards**](/help/firefly/graph/templates/storyboard-builder.md) | Neste modelo de gráfico, você constrói um storyboard cena por cena, adicionando um nó por batida da narrativa. Reordene os nós para testar uma sequência diferente antes de bloquear a ordem final dos painéis. | Comunicações e telecomunicações, bebidas, viagens |

## 3D e caractere

| Modelo de gráfico | Descrição | [!BADGE Casos de uso]{type=Informative tooltip="Casos de uso"} |
|---|---|---|
| [**Sombreadores em tempo real**](/help/firefly/graph/templates/real-time-shaders.md) | Neste modelo de gráfico, você começa com uma imagem, aplica três sombreadores personalizados diferentes e visualiza o resultado em tempo real. Ajuste os parâmetros de sombreador diretamente no nó em vez de renderizar do zero. | Técnico, automotivo e varejo |
| [**Geração de modelo de caractere**](/help/firefly/graph/templates/character-model-generation.md) | Neste modelo de gráfico, você cria um estilo animado 3D de uma ilustração. O modelo gera uma passagem de modelo 3D base pronta para ser entregue a um modelador para limpeza, em vez de iniciar a partir de uma cena em branco. | Atividades ao ar livre, tecnologia, educação |
| [**Design de brinquedo de vinil**](/help/firefly/graph/templates/vinyl-toy-design.md) | Neste modelo de gráfico, você insere uma referência de personagem ou mascote e a renderiza em uma forma estilizada de brinquedo de vinil. Há ângulos de rotação para uma plataforma de licenciamento ou revisão de produtos. | Varejo, Bebidas, Entretenimento |
| [**Virar do Sketch para 3D**](/help/firefly/graph/templates/sketch-to-3d.md) | Neste modelo de gráfico, você transforma um esboço em um caractere 3D. O gráfico cria um giro 3D giratório a partir dele, pronto para uma revisão interna de design antes de qualquer protótipo físico. | Tecnologia, Automotivo, Entretenimento |

## Modelos de produtos e marcas

| Modelo de gráfico | Descrição | [!BADGE Casos de uso]{type=Informative tooltip="Casos de uso"} |
|---|---|---|
| [**Visualização de identidade visual**](/help/firefly/graph/templates/branding-visualization.md) | Neste modelo de gráfico, saiba como visualizar o logotipo ou a marca nas cenas do produto. Alimentar as diretrizes de marca ou um logotipo e uma paleta de cores e o gráfico produz arte-chave estática e um movimento curto em uma execução, para que ambos os formatos permaneçam visualmente alinhados. | Tecnologia, bebidas, finanças |
| [**Modelo de produto da marca**](/help/firefly/graph/templates/brand-product-mockup.md) | Neste modelo de gráfico, saiba como visualizar seu produto em diferentes cenas. Você solta uma renderização de produto ou foto no nó do modelo e o gráfico a coloca dentro de uma cena totalmente da marca, com iluminação e sombra correspondentes a essa cena automaticamente. | Varejo, Bebidas, Tecnologia |
| [**Fotos editoriais**](/help/firefly/graph/templates/editorial-photoshoot.md) | Neste modelo de gráfico, carregue uma referência de modelo e troque a entrada de vestuário para cada nova aparência. Os nós de pose e iluminação permanecem bloqueados no conjunto para proporcionar uma sensação editorial consistente. | Varejo, Beleza, Atividades ao ar livre |
| [**Estúdio de fotografia**](/help/firefly/graph/templates/photography-studio.md) | Neste modelo de gráfico, você coloca uma renderização de produto no plano de fundo de estúdio e ajusta a iluminação até que o resultado se pareça com uma captura de estúdio real. | Bebidas, Tecnologia, Varejo |
| [**Aplicar decalque em superfícies**](/help/firefly/graph/templates/decal-to-surfaces.md) | Neste modelo de gráfico, você carrega o modelo do produto base e o ativo de decalque ou logotipo como entradas separadas. O modelo quebra o decalque na geometria da superfície para que siga os contornos corretamente. | Atividades ao ar livre, automotivas, varejo |

## Operações de lote e consistência

| Modelo de gráfico | Descrição | [!BADGE Casos de uso]{type=Informative tooltip="Casos de uso"} |
|---|---|---|
| [**Gerador de sistema de design**](/help/firefly/graph/templates/design-system-generator.md) | Neste modelo de gráfico, você gera um sistema de design com base em uma captura de tela do site. O gráfico produz um conjunto correspondente de ícones, padrões e componentes de layout em uma única execução em lote. | Tecnologia, finanças, comunicações e telecomunicações |
| [**Geração de headshots**](/help/firefly/graph/templates/headshots-generation.md) | Neste modelo de gráfico, você harmoniza um lote de headshots corporativos. Carregue as fotos de origem, uma por pessoa, e o gráfico normalizará a iluminação, o plano de fundo e o corte em todo o conjunto em uma execução. | Tecnologia, finanças, saúde |

Retorne ao [Introdução ao Firefly Graph](https://experienceleague.adobe.com/en/docs/creative-cloud-enterprise-learn/cce-learning-hub/fireflyoverview/firefly-graph/overview-firefly-graph).