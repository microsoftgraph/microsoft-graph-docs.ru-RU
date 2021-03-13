---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: cec38b7129eb5571544bd9c18a1e16ce875409de
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774245"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var outlookTaskFolder = new OutlookTaskFolder
{
    Name = "Cooking"
};

await graphClient.Me.Outlook.TaskGroups["{outlookTaskGroup-id}"].TaskFolders
    .Request()
    .AddAsync(outlookTaskFolder);

```