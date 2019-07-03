---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d6fd34cac6e237a97ffc4dc56b72f9e57c9099e9
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35487660"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var comment = "Cancelling for this week due to all hands";

await graphClient.Me.Events["{id}"]
    .Cancel(comment)
    .Request()
    .PostAsync();

```