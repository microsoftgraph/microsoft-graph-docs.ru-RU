---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f44abcc65f5c6efc9357c6a5d52f4c770526883c
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "53005697"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    Id = "15c1a2d5-9101-44b2-83ab-885db8a647ca"
};

await graphClient.DirectoryRoles["{directoryRole-id}"].Members.References
    .Request()
    .AddAsync(directoryObject);

```