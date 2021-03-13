---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c79ea57bb68e0b002fa0919754f6383dc17ddeb0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798724"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var allowedUsers = await graphClient.Print.Shares["{printerShare-id}"].AllowedUsers
    .Request()
    .GetAsync();

```