---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f1e40b94ebe1a223532af81cc3d1cc0f5cbdad65
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962988"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var passwordlessMicrosoftAuthenticatorAuthenticationMethod = await graphClient.Me.Authentication.PasswordlessMicrosoftAuthenticatorMethods["{passwordlessMicrosoftAuthenticatorAuthenticationMethod-id}"]
    .Request()
    .GetAsync();

```