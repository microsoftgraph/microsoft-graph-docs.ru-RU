---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 92c9d93138d4d6094c21786509b6bbbafd21e782
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772564"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var dataSource = new UserSource
{
    Email = "badguy@contoso.com"
};

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].SourceCollections["{ediscovery.sourceCollection-id}"].AdditionalSources
    .Request()
    .AddAsync(dataSource);

```