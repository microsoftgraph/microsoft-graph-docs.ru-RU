---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ccfd9081ba291351262380d599a78e7533ffa7c2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50770409"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var itemPhone = new ItemPhone
{
    Type = PhoneType.Other
};

await graphClient.Users["{user-id}"].Profile.Phones["{itemPhone-id}"]
    .Request()
    .UpdateAsync(itemPhone);

```