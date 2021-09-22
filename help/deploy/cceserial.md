---
title: Entendendo a expiração do Creative Cloud para empresas e do número de série do Acrobat
description: Entendendo a experiência de expiração do número de série para Creative Cloud para empresas e Acrobat
role: User
level: Beginner, Intermediate
exl-id: bc457be0-86dc-4e8a-b6b2-34bc76af2d21
source-git-commit: 6b819aef801e003e5a160d24ba69522cf6a7e715
workflow-type: tm+mt
source-wordcount: '848'
ht-degree: 3%

---

# Entendendo a expiração do Creative Cloud para empresas e do número de série do Acrobat

Historicamente, o Adobe emitiu números de série com nossos aplicativos (ou seja, Creative Suite, Creative Cloud para empresas, Acrobat XI, Acrobat DC) para clientes em ETLA (Enterprise Term License Agreements, contratos de licença de termo corporativo). Esses números de série têm uma data de expiração. Depois que a data de expiração for ultrapassada, o produto não funcionará mais, portanto, é importante planejar sua migração antes que seus números de série expirem. Esta página descreve as etapas necessárias para garantir que os usuários finais tenham acesso contínuo aos aplicativos e serviços de Adobe.

## Verificando seus números de série para a data de expiração

### Localize o(s) número(s) de série

As licenças por número de série associadas ao seu contrato de ETLA estão disponíveis no [site de licenciamento de Adobe](https://licensing.adobe.com/) (LWS). Siga estas instruções para exibir e baixar:

1. Faça logon no [site de licenciamento de Adobe](https://licensing.adobe.com/) (LWS) com seu Adobe ID e senha.
1. Escolha **Licenças > Recuperar números de série**.
1. Insira seu **ID de usuário final** ou **ID de implantação**.
1. (Opcional) Selecione um **Nome do produto**, **Versão do produto** ou **Plataforma** para filtrar os resultados.
1. Clique em Pesquisar.
1. O nome do produto e os números de série são exibidos.
1. (Opcional) Selecione &quot;EXPORTAR PARA CSV&quot; para baixar a lista de números de série.

![Encontre seus números de série](assets/retrieveserialnumbers.png)

### Verifique a data de expiração

O [AdobeExpiryCheck](https://helpx.adobe.com/enterprise/kb/volume-license-expiration-check.html) é um utilitário de linha de comando para os administradores de TI verificarem se os produtos de Adobe em um computador estão usando números de série que expiraram ou estão expirando. A ferramenta exibirá informações como o identificador de licenciamento de produto (LEID), o número de série criptografado e a data de expiração. Esta [página](https://helpx.adobe.com/enterprise/kb/volume-license-expiration-check.html) contém instruções sobre como baixar e usar a ferramenta em computadores Mac ou Windows.

## Compreender a experiência do usuário final antes e depois que o número de série expirar

Os aplicativos Acrobat e Creative Cloud para empresas começarão a exibir mensagens (nos aplicativos) a partir de 60 dias antes da expiração. Quando o número de série expirar, os produtos pararão de funcionar e solicitarão que o usuário execute uma ação.

### Creative Cloud para experiência corporativa

As informações a seguir descrevem a experiência do usuário final. Há um vídeo curto abaixo seguido de uma revisão da experiência do usuário final.

>[!VIDEO](https://video.tv.adobe.com/v/331746?hidetitle=true)

**Antes da expiração**

A partir de 60 dias antes da expiração do número de série, todos os aplicativos Creative Cloud para empresas exibem uma caixa de diálogo do produto ao usuário final. Essa mensagem será exibida semanalmente, até 30 dias antes da expiração, e será exibida diariamente até a data de expiração, indicando que *Sua licença está expirando. Este Adobe está usando uma licença que expira em 29 de novembro de 2020. Entre em contato com seu administrador para garantir o acesso contínuo*.

![CCE antes da mensagem de expiração](assets/cceexpiring.png)

**Após a expiração**

Quando o número de série expirar, os usuários não terão mais acesso ao Creative Cloud para aplicativos corporativos. Na primeira inicialização após a expiração, o usuário será avisado com uma caixa de diálogo informando *O número de série inserido expirou. Este produto não pode ser licenciado. Entre em contato com o Suporte ao cliente*.

![CCE após a mensagem de expiração](assets/cceafterexpire.png)

Para todas as tentativas subsequentes de iniciar os aplicativos, o usuário final será solicitado a **Fazer logon agora** seguido pela opção para criar seu próprio Adobe ID e entrar no modo de avaliação. No entanto, qualquer novo Adobe ID criado pelo usuário final não será associado às licenças da sua organização e causará confusão adicional aos usuários. Para evitar interrupções nos negócios e/ou confusão desnecessária, migre os usuários para o licenciamento por usuário nomeado antes que o(s) número(s) de série expire.

![Caixa de diálogo Fazer logon de CCE 1](assets/ccesignin1.png)

![Caixa de diálogo de logon de CCE 2](assets/ccesignin2.png)

### Experiência Acrobat

As informações a seguir descrevem a experiência do usuário final. Há um vídeo curto abaixo seguido de uma revisão da experiência do usuário final.

>[!VIDEO](https://video.tv.adobe.com/v/331749?hidetitle=true)


**Antes da expiração**

A partir de 60 dias antes da expiração do número de série, a Acrobat exibe uma mensagem pop-up no produto para o usuário final. Isso será exibido uma vez por semana até 7 dias antes do vencimento. Ele começará a ser exibido diariamente, indicando que *Sua licença da Adobe Acrobat expira em 11/30/2020. Entre em contato com o administrador para continuar usando o Acrobat sem interrupções.*

![Mensagem de expiração do Acrobat](assets/acrobatexpiring.png)

**Após a expiração**

Quando o número de série expirar, os usuários não terão mais acesso ao Acrobat. Na primeira inicialização após a expiração, o usuário será avisado com uma caixa de diálogo informando *O número de série inserido expirou. Este produto não pode ser licenciado. Entre em contato com o Suporte ao cliente.*

![Acrobat após a mensagem de expiração](assets/acrobatafterexpire.png)

Para todas as tentativas subsequentes de iniciar o Acrobat, o usuário final será solicitado a **Fazer logon agora** seguido pela opção para criar seu próprio Adobe ID e entrar no modo de avaliação. No entanto, qualquer novo Adobe ID criado pelo usuário final não será associado às licenças da sua organização e causará confusão adicional aos usuários.

![Caixa de diálogo do Acrobat Sign 1](assets/acrobatsignin1.png)

![Caixa de diálogo do Acrobat Sign 2](assets/acrobatsignin2.png)

## Entre em contato conosco se precisar de ajuda

Se tiver dúvidas sobre como usar a ferramenta [AdobeExpiryCheck](https://helpx.adobe.com/enterprise/kb/volume-license-expiration-check.html) ou precisar de ajuda para migrar da implantação de número de série para um usuário nomeado, você terá algumas opções:
* Envie um email para a equipe de integração empresarial do Adobe - **entonb@adobe.com**
* Abra um chamado de suporte em [Admin Console](https://adminconsole.adobe.com/support)
* Entre em contato com seu Gerente de conta do Adobe ou Gerente de sucesso do cliente
