---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 251138a54514fc1fdaa14f0c9458a77101ba782c15d51428b531bb85e4dfba8a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57271530"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = new Group
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id", "https://graph.microsoft.com/beta/groups/{id}"}
    }
};

await graphClient.Print.Shares["{printerShare-id}"].AllowedGroups.References
    .Request()
    .AddAsync(group);

```