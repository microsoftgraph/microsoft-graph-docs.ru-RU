---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a8eaf5628b438370565ac816b8adf57f3ce79d7a
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34439528"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityAction = new SecurityAction
{
    Name = "BlockIp",
    ActionReason = "Test",
    Parameters = new List<KeyValuePair>()
    {
        new KeyValuePair
        {
            Name = "IP",
            Value = "1.2.3.4"
        }
    },
    VendorInformation = new SecurityVendorInformation
    {
        Provider = "Windows Defender ATP",
        Vendor = "Microsoft"
    }
};

await graphClient.Security.SecurityActions
    .Request()
    .AddAsync(securityAction);

```