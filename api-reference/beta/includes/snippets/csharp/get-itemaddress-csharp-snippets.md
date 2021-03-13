---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6bf78ac744fb383cc8d35955eac74843a00a03bb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788966"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var itemAddress = await graphClient.Me.Profile.Addresses["{itemAddress-id}"]
    .Request()
    .GetAsync();

```