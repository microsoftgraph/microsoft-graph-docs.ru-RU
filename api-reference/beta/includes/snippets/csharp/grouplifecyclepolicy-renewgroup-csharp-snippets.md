---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b347e434bf3500bcc418965cef5de340baf71a3d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35489400"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupId = "ffffffff-ffff-ffff-ffff-ffffffffffff";

await graphClient.GroupLifecyclePolicies
    .RenewGroup(groupId)
    .Request()
    .PostAsync();

```