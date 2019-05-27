---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 194e3903db818eabd3f131d1bef3d0c56846bf69
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34482614"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var synchronizationTemplate = new SynchronizationTemplate
{
    Id = "Slack",
    ApplicationId = "{id}",
    FactoryTag = "CustomSCIM"
};

await graphClient.Applications["{id}"].Synchronization.Templates["{templateId}"]
    .Request()
    .Header("Authorization","Bearer <token>")
    .PutAsync(synchronizationTemplate);

```