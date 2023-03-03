---
title: Noções básicas sobre a expiração do número de série do Creative Cloud para corporações e Acrobat
description: Entendendo a experiência de expiração de número de série para Creative Cloud para corporações e Acrobat
role: User
level: Beginner, Intermediate
exl-id: bc457be0-86dc-4e8a-b6b2-34bc76af2d21
source-git-commit: 524d071b6f4e059823601381f04c337aedc55970
workflow-type: tm+mt
source-wordcount: '844'
ht-degree: 3%

---

# Noções básicas sobre a expiração do número de série do Creative Cloud para corporações e Acrobat

Historicamente, o Adobe emitia números de série com nossos aplicativos (por exemplo, Creative Suite, Creative Cloud para corporações, Acrobat XI, Acrobat DC) para clientes em contratos de licença por período corporativo (ETLA). Esses números de série têm uma data de expiração. Após a data de expiração, o produto não funcionará mais, portanto, é importante planejar a migração antes que os números de série expirem. Esta página descreve as etapas necessárias para garantir que os usuários finais tenham acesso contínuo aos aplicativos e serviços do Adobe.

## Verificando os números de série para a data de expiração

### Localizar seus números de série

As licenças por número de série associadas ao seu contrato ETLA estão disponíveis por meio do [Site de licenciamento do Adobe](https://licensing.adobe.com/) (LWS) Siga estas instruções para exibir e baixar:

1. Fazer logon em [Site de licenciamento do Adobe](https://licensing.adobe.com/) (LWS) com sua Adobe ID e senha.
1. Escolha **Licenças > Recuperar números de série**.
1. Insira seu **ID do usuário final** ou **ID de implantação**.
1. (Opcional) Selecione um **Nome do produto**, **Versão do produto** ou **Plataforma** para filtrar resultados.
1. Clique em Pesquisar.
1. O nome do produto e os números de série são exibidos.
1. (Opcional) Selecione &quot;EXPORTAR PARA CSV&quot; para baixar a lista de números de série.

![Localizar os números de série](assets/retrieveserialnumbers.png)

### Verificar a data de expiração

O [AdobeExpiryCheck](https://helpx.adobe.com/enterprise/kb/volume-license-expiration-check.html) O é um utilitário de linha de comando para administradores de TI para verificar se os produtos Adobe em um computador estão usando números de série que expiraram ou estão expirando. A ferramenta exibirá informações como o identificador da licença do produto (LEID), o número de série criptografado e a data de expiração. Este [página](https://helpx.adobe.com/enterprise/kb/volume-license-expiration-check.html) contém instruções sobre como baixar e usar a ferramenta em computadores Mac ou Windows.

## Entender a experiência do usuário final antes e depois da expiração do número de série

Os aplicativos Acrobat e Creative Cloud para empresas começarão a exibir mensagens (nos aplicativos) a partir de 60 dias antes da expiração. Quando o número de série expira, os produtos param de funcionar e solicitam que o usuário execute uma ação.

### Creative Cloud para a experiência corporativa

As informações a seguir descrevem a experiência do usuário final. Há um breve vídeo abaixo seguido pela revisão da experiência do usuário final.

>[!VIDEO](https://video.tv.adobe.com/v/331746?hidetitle=true)

**Antes da expiração**

A partir de 60 dias antes do número de série expirar, todos os aplicativos Creative Cloud para corporações exibirão uma caixa de diálogo no produto para o usuário final. Esta mensagem será exibida semanalmente, até 30 dias antes da expiração, e então será exibida diariamente até a data de expiração *Sua licença está expirando. Este produto Adobe está usando uma licença que expira em 29 de novembro de 2020. Entre em contato com seu administrador para garantir o acesso contínuo*.

![mensagem de CCE antes da expiração](assets/cceexpiring.png)

**Após a expiração**

Depois que o número de série expirar, os usuários não terão mais acesso ao Creative Cloud para aplicativos corporativos. Na primeira inicialização após a expiração, o usuário receberá uma caixa de diálogo informando *O número de série inserido expirou. Este produto não pode ser licenciado. Entre em contato com o Suporte ao cliente*.

![Mensagem de expiração de CCE](assets/cceafterexpire.png)

Em todas as tentativas subsequentes de iniciar os aplicativos, o usuário final será solicitado a **Fazer logon agora** seguido pela opção de criar seu próprio Adobe ID e entrar no modo de avaliação. No entanto, qualquer novo Adobe ID criado pelo usuário final não será associado às licenças da sua organização e causará confusão adicional aos usuários. Para evitar interrupções nos negócios e/ou confusão desnecessária, migre seus usuários para o licenciamento por usuário nomeado antes que seus números de série expirem.

![Caixa de diálogo de logon do CCE 1](assets/ccesignin1.png)

![Caixa de diálogo de logon 2 do CCE](assets/ccesignin2.png)

### Experiência com o Acrobat

As informações a seguir descrevem a experiência do usuário final. Há um breve vídeo abaixo seguido pela revisão da experiência do usuário final.

>[!VIDEO](https://video.tv.adobe.com/v/331749?hidetitle=true)


**Antes da expiração**

A partir de 60 dias antes do número de série expirar, o Acrobat exibe uma mensagem pop-up no produto para o usuário final. Isso aparecerá uma vez por semana até 7 dias antes do vencimento. Começará então a aparecer diariamente declarando *Sua licença do Adobe Acrobat expira em 11/30/2020. Entre em contato com o administrador para continuar usando o Acrobat sem interrupções.*

![Mensagem de expiração do Acrobat](assets/acrobatexpiring.png)

**Após a expiração**

Quando o número de série expirar, os usuários não terão mais acesso ao Acrobat. Na primeira inicialização após a expiração, o usuário receberá uma caixa de diálogo informando *O número de série inserido expirou. Este produto não pode ser licenciado. Entre em contato com o Suporte ao cliente.*

![Acrobat após mensagem de expiração](assets/acrobatafterexpire.png)

Em todas as tentativas subsequentes de iniciar o Acrobat, o usuário final será solicitado a **Fazer logon agora** seguido pela opção de criar seu próprio Adobe ID e entrar no modo de avaliação. No entanto, qualquer novo Adobe ID criado pelo usuário final não será associado às licenças da sua organização e causará confusão adicional aos usuários.

![Acrobat Sign no diálogo 1](assets/acrobatsignin1.png)

![Acrobat Sign no diálogo 2](assets/acrobatsignin2.png)

## Entre em contato se precisar de ajuda

Se tiver dúvidas sobre como usar o [AdobeExpiryCheck](https://helpx.adobe.com/enterprise/kb/volume-license-expiration-check.html) ou precisar de ajuda para migrar da implantação do número de série para o usuário nomeado, você tem algumas opções:
* Envie um email para a equipe de integração corporativa do Adobe - **entonb@adobe.com**
* Abra um tíquete de suporte no [Admin Console](https://adminconsole.adobe.com/support)
* Entre em contato com a equipe de conta da Adobe
