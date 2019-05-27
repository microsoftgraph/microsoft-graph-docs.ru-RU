---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 19e7f26a82c30f51364534dfe768f5ec2e981ceb
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34443791"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupIds = new List<String>()
{
    "groupIds-value"
};

await graphClient.Contacts["{id}"]
    .CheckMemberGroups(groupIds)
    .Request()
    .PostAsync();

```