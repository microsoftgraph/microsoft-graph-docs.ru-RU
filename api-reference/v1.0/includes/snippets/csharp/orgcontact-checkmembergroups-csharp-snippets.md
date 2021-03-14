---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6a2f12be35c981aecb4e9e00ecf6854d77699ea5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787813"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupIds = new List<String>()
{
    "groupId-value1",
    "groupId-value2"
};

await graphClient.Contacts["{orgContact-id}"]
    .CheckMemberGroups(groupIds)
    .Request()
    .PostAsync();

```