---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a1ec222a0037dd97728bc767bbc2cc992dc7a7c8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799088"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var longRunningOperation = await graphClient.Users["{user-id}"].Authentication.Operations["{longRunningOperation-id}"]
    .Request()
    .GetAsync();

```