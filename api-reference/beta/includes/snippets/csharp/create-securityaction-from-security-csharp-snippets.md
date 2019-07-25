---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a8eaf5628b438370565ac816b8adf57f3ce79d7a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725426"
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