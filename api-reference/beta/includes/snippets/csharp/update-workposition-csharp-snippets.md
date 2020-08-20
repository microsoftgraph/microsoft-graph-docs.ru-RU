---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5d66060d252eedd985635387cb400a4d6c86f054
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/20/2020
ms.locfileid: "46821017"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workPosition = new WorkPosition
{
    IsCurrent = true
};

await graphClient.Me.Profile.Positions["{id}"]
    .Request()
    .UpdateAsync(workPosition);

```