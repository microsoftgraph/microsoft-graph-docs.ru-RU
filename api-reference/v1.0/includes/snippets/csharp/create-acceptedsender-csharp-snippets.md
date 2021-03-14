---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c2be8bd9231a6eca4d93353bc0390f62ffa23d25
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781063"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    Id = "alexd@contoso.com"
};

await graphClient.Groups["{group-id}"].AcceptedSenders.References
    .Request()
    .AddAsync(directoryObject);

```