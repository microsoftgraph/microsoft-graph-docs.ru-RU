---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 20efc75d238e06b807e50b22e2332f2974900902
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48604736"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupSetting = await graphClient.GroupSettings["{id}"]
    .Request()
    .GetAsync();

```