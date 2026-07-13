---
title: ​3. Crie seu primeiro gráfico
description: Um passo a passo para criar seu primeiro fluxo de trabalho do Firefly Graph
feature: Image Editing, Gen AI
role: User
level: Beginner
jira: KT-
hide: true
hidefromtoc: true
source-git-commit: 4dd919a2b06f0852dc0010b0f79d5a0b2eae4c1a
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 1%

---

# &#x200B;3. Crie seu primeiro gráfico

Assim que souber o que são um nó, uma conexão e um modelo, você estará pronto para criar seu primeiro fluxo de trabalho.

1. Abra o Firefly e selecione **Gráfico** no menu à esquerda.
1. Selecione **Criar novo gráfico**.
1. Clique com o botão direito na tela em branco e selecione mais de **novo nó**.
1. Selecione **Entrada** no menu à esquerda, depois **Imagem de Entrada**.
   ![Nó](../assets/node.png)
Este é um nó que permite importar um gráfico.
1. Arraste e solte uma imagem no nó.
   ![Nó com imagem](../assets/node-image.png)
1. Clique com o botão direito na tela em branco e selecione **+ novo nó** e selecione **Máscara de Gradiente** na caixa de diálogo.
1. Clique com o botão direito na tela em branco e selecione **+ novo nó** e selecione **Aplicar máscara** na caixa de diálogo.
1. Conecte a saída do nó **Imagem de entrada** à entrada do nó de imagem **Aplicar máscara**.
1. Conecte a saída da **Máscara de gradiente** à entrada de canal/máscara **Aplicar máscara**.
   ![Nós de plug-in](../assets/plug-in.png)

## Próxima etapa

Começando com um modelo? Vá para [4. Personalize um modelo ](https://experienceleague.adobe.com/en/docs/creative-cloud-enterprise-learn/cce-learning-hub/fireflyoverview/firefly-graph/customize-template) para que ele reflita seu próprio resumo.
