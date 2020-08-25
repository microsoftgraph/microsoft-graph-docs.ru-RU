---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5872b89989126a9de9aa6d2b91eda5c6a1c41e21
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873915"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var used = await graphClient.Me.Insights.Used
    .Request()
    .OrderBy("LastUsed/LastAccessedDateTime desc")
    .GetAsync();

```