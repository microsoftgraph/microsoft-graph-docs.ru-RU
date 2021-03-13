---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6a4048ef47c53f941e298b5a00a2b555bb21c400
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778961"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var outlookTaskGroup = await graphClient.Me.Outlook.TaskGroups["{outlookTaskGroup-id}"]
    .Request()
    .GetAsync();

```