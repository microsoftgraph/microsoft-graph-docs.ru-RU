---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 98545914a0c0bfc108a1ad69437dfce07749548a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772459"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var account = await graphClient.Me.Profile.Account
    .Request()
    .GetAsync();

```