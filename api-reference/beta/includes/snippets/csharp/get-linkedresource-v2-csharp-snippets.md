---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a62daf50d6de31ad480989aa7185a2ff35ae3fbf
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62099599"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var linkedResource_v2 = await graphClient.Me.Tasks.Lists["{baseTaskList-id}"].Tasks["{baseTask-id}"].LinkedResources["{linkedResource_v2-id}"]
    .Request()
    .GetAsync();

```