---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 971545faba675f855c05a820df814d794222c319
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34448088"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var outlookTaskFolder = await graphClient.Me.Outlook.TaskFolders["AAMkADIyAAAAABrJAAA="]
    .Request()
    .GetAsync();

```