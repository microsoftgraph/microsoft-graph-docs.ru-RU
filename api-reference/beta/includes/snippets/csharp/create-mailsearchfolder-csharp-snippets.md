---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c8a963a14c2a6aaf988bf1fcc8e2daa27586ae53
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801012"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mailFolder = new MailSearchFolder
{
    DisplayName = "Weekly digests",
    IncludeNestedFolders = true,
    SourceFolderIds = new List<String>()
    {
        "AQMkADYAAAIBDAAAAA=="
    },
    FilterQuery = "contains(subject, 'weekly digest')"
};

await graphClient.Me.MailFolders["{mailFolder-id}"].ChildFolders
    .Request()
    .AddAsync(mailFolder);

```