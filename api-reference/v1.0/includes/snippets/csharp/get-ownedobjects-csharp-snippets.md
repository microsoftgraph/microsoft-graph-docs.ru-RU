---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2959b6731cceca6353c3a0c160ed0881e20d36e2
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35734297"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ownedObjects = await graphClient.Me.OwnedObjects
    .Request()
    .GetAsync();

```