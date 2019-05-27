---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 86f2fcf768faf1a77d30dd3eafc098b94b19f6c8
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34479345"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupLifecyclePolicy = new GroupLifecyclePolicy
{
    GroupLifetimeInDays = 180,
    ManagedGroupTypes = "Selected",
    AlternateNotificationEmails = "admin@contoso.com"
};

await graphClient.GroupLifecyclePolicies["{id}"]
    .Request()
    .UpdateAsync(groupLifecyclePolicy);

```