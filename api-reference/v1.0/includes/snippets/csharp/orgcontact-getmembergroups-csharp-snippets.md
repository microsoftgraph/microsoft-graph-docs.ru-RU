---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1809054297f25384b67da95a071bbfce96edeae7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778852"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityEnabledOnly = false;

await graphClient.Contacts["{orgContact-id}"]
    .GetMemberGroups(securityEnabledOnly)
    .Request()
    .PostAsync();

```