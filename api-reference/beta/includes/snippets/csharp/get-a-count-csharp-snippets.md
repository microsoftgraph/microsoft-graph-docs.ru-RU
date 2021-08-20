---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3b0291972845bb717865d129ea25336b84edc862
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58369135"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contacts = await graphClient.Contacts
    .Request()
    .Header("ConsistencyLevel","eventual")
    .Filter("startswith(displayName,'A')")
    .OrderBy("displayName")
    .Top(1)
    .GetAsync();

```