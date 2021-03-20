---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4ac215f36ae2b9c402bdfbacf5104a7bad97ef23
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50946838"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var usageRights = await graphClient.Devices["{device-id}"].UsageRights
    .Request()
    .Filter("state in ('active', 'suspended') and serviceIdentifier in ('ABCD')")
    .GetAsync();

```