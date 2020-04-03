---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 29efcb266954cb7d3326fc679fb2d6cb9b479173
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2020
ms.locfileid: "43124891"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var recipients = new List<DriveRecipient>()
{
    new DriveRecipient
    {
        Email = "john@contoso.com"
    },
    new DriveRecipient
    {
        Email = "ryan@external.com"
    }
};

var roles = new List<String>()
{
    "read"
};

await graphClient.Shares["{encoded-sharing-url}"].Permission
    .Grant(roles,recipients)
    .Request()
    .PostAsync();

```