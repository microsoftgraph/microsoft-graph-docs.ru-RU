---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0f3d3ebb482b39074b644177fea19ed5c8cfd8d2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788262"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityApiConnector = new IdentityApiConnector
{
    DisplayName = "New Test API",
    TargetUrl = "https://otherapi.com/api/endpoint",
    AuthenticationConfiguration = new BasicAuthentication
    {
        Username = "<NEW_USERNAME>",
        Password = "<NEW_PASSWORD>"
    }
};

await graphClient.Identity.ApiConnectors["{identityApiConnector-id}"]
    .Request()
    .UpdateAsync(identityApiConnector);

```