---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2fa44c20e4cb737f3ad97cd344d57abbc718cd9e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "60927070"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var noncustodialDataSource = new Microsoft.Graph.Ediscovery.NoncustodialDataSource
{
    ApplyHoldToSource = false,
    DataSource = new SiteSource
    {
        Site = new Site
        {
            WebUrl = "https://contoso.sharepoint.com/sites/SecretSite"
        }
    }
};

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].NoncustodialDataSources
    .Request()
    .AddAsync(noncustodialDataSource);

```