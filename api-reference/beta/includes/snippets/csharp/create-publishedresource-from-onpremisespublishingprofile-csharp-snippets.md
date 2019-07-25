---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: cbb431c9bca98cc811571c444c1b045aa0c62f5f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875044"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var publishedResource = new PublishedResource
{
    DisplayName = "New provisioning",
    ResourceName = "domain1.contoso.com"
};

await graphClient.OnPremisesPublishingProfiles["provisioning"].PublishedResources
    .Request()
    .AddAsync(publishedResource);

```