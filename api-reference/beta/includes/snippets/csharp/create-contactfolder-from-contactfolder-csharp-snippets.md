---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f6c68978687948a98eb0c99c08b4a305128290b7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809679"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contactFolder = new ContactFolder
{
    DisplayName = "displayName-value"
};

await graphClient.Me.ContactFolders["{contactFolder-id}"].ChildFolders
    .Request()
    .AddAsync(contactFolder);

```