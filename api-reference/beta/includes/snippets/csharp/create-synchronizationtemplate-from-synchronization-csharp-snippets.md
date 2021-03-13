---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4b2b5b3687f7e17ca5c26b43dbfb2b629ef392c2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775446"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var synchronizationTemplate = new SynchronizationTemplate
{
    Id = "SCIM-Test1",
    ApplicationId = Guid.Parse("{id}"),
    FactoryTag = "CustomSCIM"
};

await graphClient.Applications["{application-id}"].Synchronization.Templates
    .Request()
    .AddAsync(synchronizationTemplate);

```