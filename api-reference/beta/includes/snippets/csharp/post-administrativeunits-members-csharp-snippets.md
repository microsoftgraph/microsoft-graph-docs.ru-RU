---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e6615be9136e888cc3f21948482a58261258c41d
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890252"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new Group
{
    Description = "Self help community for golf",
    DisplayName = "Golf Assist",
    GroupTypes = new List<String>()
    {
        "Unified"
    },
    MailEnabled = true,
    MailNickname = "golfassist",
    SecurityEnabled = false
};

await graphClient.AdministrativeUnits["{administrativeUnit-id}"].Members
    .Request()
    .AddAsync(directoryObject);

```