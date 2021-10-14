---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9220b611744bfe78af4f82855dcb83ad09998fe794782d02294035505e6037cd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57052763"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupIds = new List<String>()
{
    "groupIds-value"
};

await graphClient.Contacts["{orgContact-id}"]
    .CheckMemberGroups(groupIds)
    .Request()
    .PostAsync();

```