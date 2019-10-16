---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 685aadaf1f2daf806a5e4dde040423958bcff889
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37544461"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var post = new Post
{
    Body = new ItemBody
    {
        ContentType = BodyType.Text,
        Content = "I attached a reference to a file on OneDrive."
    },
    Attachments = new List<Attachment>()
    {
        new ReferenceAttachment
        {
            Name = "Personal pictures",
            SourceUrl = "https://contoso.com/personal/mario_contoso_net/Documents/Pics",
            ProviderType = "oneDriveConsumer",
            Permission = "Edit",
            IsFolder = "True"
        }
    }
};

await graphClient.Groups["1848753d-185d-4c08-a4e4-6ee40521d115"].Threads["AAQkADJUdfolA=="]
    .Reply(post)
    .Request()
    .PostAsync();

```