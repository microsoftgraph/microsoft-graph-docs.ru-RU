---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2959b6731cceca6353c3a0c160ed0881e20d36e2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960526"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ownedObjects = await graphClient.Me.OwnedObjects
    .Request()
    .GetAsync();

```