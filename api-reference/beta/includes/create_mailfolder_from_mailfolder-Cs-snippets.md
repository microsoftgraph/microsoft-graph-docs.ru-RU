---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 06f7aab4f4e38d8a2fda4a6a5bc22e807b4826d7
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34466481"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mailFolder = new MailFolder
{
    DisplayName = "displayName-value"
};

await graphClient.Me.MailFolders["{id}"].ChildFolders
    .Request()
    .AddAsync(mailFolder);

```