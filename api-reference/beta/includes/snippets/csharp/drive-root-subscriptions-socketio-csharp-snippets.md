---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 21ab5b4454c31f3299eb676dfbfe6d96c066309b
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48616242"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var subscription = await graphClient.Me.Drive.Root.Subscriptions["socketIo"]
    .Request()
    .GetAsync();

```