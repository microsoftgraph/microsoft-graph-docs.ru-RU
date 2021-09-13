---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f8f69c3b2b0bcfcbb2db14741e67c9ea195d5356fbe2b90cf4f2e78e22a316c4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57321841"
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