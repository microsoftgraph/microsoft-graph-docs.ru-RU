---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3d90486f9d385c43f84cdc3a41f321d15394ed90
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807324"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityEnabledOnly = true;

await graphClient.DirectoryObjects["{directoryObject-id}"]
    .GetMemberGroups(securityEnabledOnly)
    .Request()
    .PostAsync();

```