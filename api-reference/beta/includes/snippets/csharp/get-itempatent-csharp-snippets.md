---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 69a405fa4bb39d21ff864a2a7d36ee92564fe198
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798995"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var itemPatent = await graphClient.Me.Profile.Patents["{itemPatent-id}"]
    .Request()
    .GetAsync();

```