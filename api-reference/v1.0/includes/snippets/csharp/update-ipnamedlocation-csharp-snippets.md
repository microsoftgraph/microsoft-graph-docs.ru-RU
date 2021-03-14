---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6c5cb930a4cd09ef9743820fa048b0d1283c7cd0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795926"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var namedLocation = new IpNamedLocation
{
    DisplayName = "Untrusted named location with only IPv4 address",
    IsTrusted = false,
    IpRanges = new List<IpRange>()
    {
        new IPv4CidrRange
        {
            CidrAddress = "6.5.4.3/18"
        }
    }
};

await graphClient.Identity.ConditionalAccess.NamedLocations["{namedLocation-id}"]
    .Request()
    .UpdateAsync(namedLocation);

```