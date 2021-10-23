---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e67dcc9024b781c8c744678dc9bf44cafa488f61
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2021
ms.locfileid: "60561544"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var organizationalBranding = new OrganizationalBranding
{
    SignInPageText = "Default",
    UsernameHintText = "DefaultHint"
};

await graphClient.Organization["{organization-id}"].Branding
    .Request()
    .Header("Accept-Language","0")
    .UpdateAsync(organizationalBranding);

```