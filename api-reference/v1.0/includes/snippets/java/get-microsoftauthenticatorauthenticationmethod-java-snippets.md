---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 09e3a388874c48b4d3b4a3b753d0fea5cec12eb667596d1d2e22e580d20a4cfa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57430675"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MicrosoftAuthenticatorAuthenticationMethod microsoftAuthenticatorAuthenticationMethod = graphClient.users("anirban@contoso.com").authentication().microsoftAuthenticatorMethods("_jpuR-TGZtk6aQCLF3BQjA2")
    .buildRequest()
    .get();

```