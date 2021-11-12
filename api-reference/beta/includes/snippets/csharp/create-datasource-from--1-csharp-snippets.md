---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fbe4274ce7be5626536ce7ced176c6b22ba1d5ff
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "60936884"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var dataSource = new SiteSource
{
    Site = new Site
    {
        WebUrl = "https://contoso.sharepoint.com/sites/SecretSite"
    }
};

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].SourceCollections["{ediscovery.sourceCollection-id}"].AdditionalSources
    .Request()
    .AddAsync(dataSource);

```