---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b2701e3eff14402ae8b67c27466890ebeadb3252
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804781"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var extension = await graphClient.Me.Messages["{message-id}"].Extensions["{extension-id}"]
    .Request()
    .GetAsync();

```