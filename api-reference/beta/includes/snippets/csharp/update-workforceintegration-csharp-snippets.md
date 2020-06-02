---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f4c73000999717c36531b9ddb7e69f282a81f826
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "40870469"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workforceIntegrations = new WorkforceIntegration
{
    DisplayName = "displayName-value",
    ApiVersion = 99,
    Encryption = new WorkforceIntegrationEncryption
    {
        Protocol = WorkforceIntegrationEncryptionProtocol.SharedSecret,
        Secret = "secret-value"
    },
    IsActive = true,
    Url = "url-value",
    Supports = WorkforceIntegrationSupportedEntities.None
};

await graphClient.Teamwork.WorkforceIntegrations
    .Request()
    .UpdateAsync(workforceIntegrations);

```