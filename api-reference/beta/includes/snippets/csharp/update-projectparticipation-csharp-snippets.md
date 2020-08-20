---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2288de0c0abdf1eea6ebe43fa113f4b4090549e4
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/20/2020
ms.locfileid: "46821264"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var projectParticipation = new ProjectParticipation
{
    AllowedAudiences = AllowedAudiences.Organization,
    Client = new CompanyDetail
    {
        Department = "Corporate Marketing",
        WebUrl = "https://www.contoso.com"
    }
};

await graphClient.Me.Profile.Projects["{id}"]
    .Request()
    .UpdateAsync(projectParticipation);

```