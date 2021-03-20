---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 14c13fa8de334334526aae26ad56ae48900f90d8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50946121"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userSource = new Microsoft.Graph.Ediscovery.UserSource
{
    Email = "megan@contoso.com",
    IncludedSources = Microsoft.Graph.Ediscovery.SourceType.Mailbox | Microsoft.Graph.Ediscovery.SourceType.Site
};

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].Custodians["{ediscovery.custodian-id}"].UserSources
    .Request()
    .AddAsync(userSource);

```