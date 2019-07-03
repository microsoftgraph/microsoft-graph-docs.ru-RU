---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 791ff036fd126621b2820653633f01f25b3f8710
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35488947"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contactFolder = new ContactFolder
{
    DisplayName = "displayName-value"
};

await graphClient.Me.ContactFolders["{id}"].ChildFolders
    .Request()
    .AddAsync(contactFolder);

```