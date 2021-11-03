---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 50e11e49e6fc9b77949ec6b3f0dc814140623b79
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696369"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authoredNote = new AuthoredNote
{
    Content = new ItemBody
    {
        Content = "String",
        ContentType = BodyType.Text
    }
};

await graphClient.Privacy.SubjectRightsRequests["{subjectRightsRequest-id}"].Notes
    .Request()
    .AddAsync(authoredNote);

```