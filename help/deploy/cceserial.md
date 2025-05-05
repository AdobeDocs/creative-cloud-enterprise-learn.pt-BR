---
title: Entendendo a expiração do Creative Cloud para corporações e do número de série do Acrobat
description: Experiência de expiração do número de série para Creative Cloud para corporações e Acrobat
role: Admin
level: Beginner, Intermediate
feature: Deploy
exl-id: bc457be0-86dc-4e8a-b6b2-34bc76af2d21
source-git-commit: c57212d39b2e613964bc15d2967a1958dc0c8c8e
workflow-type: tm+mt
source-wordcount: '840'
ht-degree: 1%

---

# Entendendo a expiração do Creative Cloud para corporações e do número de série do Acrobat

Historicamente, a Adobe emitia números de série com nossos aplicativos (por exemplo, Creative Suite, Creative Cloud para corporações, Acrobat XI, Acrobat DC) para clientes em Contratos de Licença de Termo Corporativos (ETLA). Esses números de série têm uma data de expiração. Depois que a data de expiração terminar, o produto não funcionará mais, portanto, é importante planejar a migração antes que os números de série expirem. Esta página descreve as etapas necessárias para garantir que os usuários finais tenham acesso contínuo aos aplicativos e serviços do Adobe.

## Verificando os números de série em busca da data de expiração

### Localizar o(s) número(s) de série

As licenças por número de série associadas ao seu contrato ETLA estão disponíveis no [Site de Licenciamento por Adobe](https://licensing.adobe.com/) (LWS). Siga estas instruções para exibir e baixar:

1. Entre no [site de licenciamento de Adobe](https://licensing.adobe.com/) (LWS) com sua Adobe ID e senha.
1. Escolha **Licenças > Recuperar Números de Série**.
1. Insira sua **ID de Usuário Final** ou **ID de Implantação**.
1. (Opcional) Selecione um **Nome do Produto**, uma **Versão do Produto** ou uma **Plataforma** para filtrar os resultados.
1. Clique em Pesquisar.
1. O nome do produto e os números de série são exibidos.
1. (Opcional) Selecione “EXPORTAR PARA CSV” para baixar a lista de números de série.

![Localizar seus números de série](assets/retrieveserialnumbers.png)

### Verificar a data de expiração

O [AdobeExpiryCheck](https://helpx.adobe.com/br/enterprise/kb/volume-license-expiration-check.html) é um utilitário de linha de comando para administradores de TI para verificar se os produtos Adobe em um computador estão usando números de série que expiraram ou estão expirando. A ferramenta exibirá informações como o identificador da licença do produto (LEID), o número de série criptografado e a data de expiração. Esta [página](https://helpx.adobe.com/br/enterprise/kb/volume-license-expiration-check.html) contém instruções sobre como baixar e usar a ferramenta em computadores Mac ou Windows.

## Entendendo a experiência do usuário final antes e depois da expiração do número de série

Os aplicativos da Acrobat e da Creative Cloud para corporações começarão a exibir mensagens (nos aplicativos) a partir de 60 dias antes da expiração. Depois que o número de série expira, os produtos param de funcionar e solicitam que o usuário tome medidas.

### Creative Cloud para a experiência corporativa

As informações a seguir descrevem a experiência do usuário final. Há um breve vídeo abaixo seguido pela análise da experiência do usuário final.

>[!VIDEO](https://video.tv.adobe.com/v/331746?hidetitle=true)

**Antes da expiração**

A partir de 60 dias antes do número de série expirar, todos os Creative Cloud para aplicativos corporativos exibirão uma caixa de diálogo no produto para o usuário final. Esta mensagem será exibida semanalmente, até 30 dias antes da expiração. Ela será exibida diariamente até a data de expiração que começa com *Sua licença está expirando. Este produto Adobe está usando uma licença que expira em 29 de novembro de 2020. Entre em contato com o administrador para garantir o acesso contínuo*.

![Mensagem de CCE antes da expiração](assets/cceexpiring.png)

**Após a expiração**

Depois que o número de série expirar, os usuários não terão mais acesso ao Creative Cloud para aplicativos corporativos. Na primeira inicialização após a expiração, o usuário receberá uma caixa de diálogo informando *O número de série inserido expirou. Este produto não pode ser licenciado. Contate o Suporte ao Cliente*.

![Mensagem de CCE após expiração](assets/cceafterexpire.png)

Para todas as tentativas subsequentes de iniciar os aplicativos, o usuário final será solicitado a **Fazer logon agora**, seguido da opção de criar sua própria Adobe ID e entrar no modo de avaliação. No entanto, qualquer novo Adobe ID criado pelo usuário final não será associado às licenças da sua organização e causará confusão adicional aos seus usuários. Para evitar a interrupção dos negócios e/ou confusões desnecessárias, migre seus usuários para o licenciamento por usuário nomeado antes que os números de série expirem.

![Caixa de diálogo de entrada do CCE 1](assets/ccesignin1.png)

![Caixa de diálogo de entrada do CCE 2](assets/ccesignin2.png)

### experiência com Acrobat

As informações a seguir descrevem a experiência do usuário final. Há um breve vídeo abaixo seguido pela análise da experiência do usuário final.

>[!VIDEO](https://video.tv.adobe.com/v/331749?hidetitle=true)


**Antes da expiração**

A partir de 60 dias antes do número de série expirar, o Acrobat exibe uma mensagem pop-up no produto para o usuário final. Isso será exibido uma vez por semana até 7 dias antes do vencimento. Ela começará a aparecer diariamente a partir de *Sua licença do Adobe Acrobat expira em 11/30/2020. Entre em contato com o administrador para continuar usando o Acrobat sem interrupções.*

![Mensagem de expiração do Acrobat](assets/acrobatexpiring.png)

**Após a expiração**

Depois que o número de série expirar, os usuários não terão mais acesso ao Acrobat. Na primeira inicialização após a expiração, o usuário receberá uma caixa de diálogo informando *O número de série inserido expirou. Este produto não pode ser licenciado. Entre em contato com o Suporte ao Cliente.*

![Mensagem sobre o Acrobat após a expiração](assets/acrobatafterexpire.png)

Para todas as tentativas subsequentes de iniciar o Acrobat, o usuário final será solicitado a **Fazer logon agora** seguido da opção de criar sua própria Adobe ID e entrar no modo de avaliação. No entanto, qualquer novo Adobe ID criado pelo usuário final não será associado às licenças da sua organização e causará confusão adicional aos seus usuários.

![Acrobat Sign na caixa de diálogo 1](assets/acrobatsignin1.png)

![Acrobat Sign na caixa de diálogo 2](assets/acrobatsignin2.png)

## Fale conosco se precisar de ajuda

Se você tiver dúvidas sobre como usar a ferramenta [AdobeExpiryCheck](https://helpx.adobe.com/br/enterprise/kb/volume-license-expiration-check.html) ou precisar de ajuda para migrar da implantação de número de série para um usuário nomeado, terá algumas opções:
* Enviar um email para a equipe de integração do Adobe Enterprise - **entonb@adobe.com**
* Abrir um tíquete de suporte em [Admin Console](https://adminconsole.adobe.com/support)
* Entre em contato com sua equipe de conta do Adobe
