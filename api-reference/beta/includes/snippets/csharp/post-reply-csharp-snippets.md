---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 28709f94dd32756d2d41fe1bdca0de05ebd0bc72
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793988"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var post = new Post
{
    Body = new ItemBody
    {
        ContentType = BodyType.Text,
        Content = "content-value"
    },
    ReceivedDateTime = DateTimeOffset.Parse("2016-10-19T10:37:00Z"),
    HasAttachments = true,
    From = new Recipient
    {
        EmailAddress = new EmailAddress
        {
            Name = "name-value",
            Address = "address-value"
        }
    },
    Sender = new Recipient
    {
        EmailAddress = new EmailAddress
        {
            Name = "name-value",
            Address = "address-value"
        }
    },
    ConversationThreadId = "conversationThreadId-value",
    NewParticipants = new List<Recipient>()
    {
        new Recipient
        {
            EmailAddress = new EmailAddress
            {
                Name = "name-value",
                Address = "address-value"
            }
        }
    },
    ConversationId = "conversationId-value",
    CreatedDateTime = DateTimeOffset.Parse("2016-10-19T10:37:00Z"),
    LastModifiedDateTime = DateTimeOffset.Parse("2016-10-19T10:37:00Z"),
    ChangeKey = "changeKey-value",
    Categories = new List<String>()
    {
        "categories-value"
    },
    Id = "id-value",
    InReplyTo = new Post
    {
    },
    Attachments = new PostAttachmentsCollectionPage()
    {
        new FileAttachment
        {
            LastModifiedDateTime = DateTimeOffset.Parse("2016-10-19T10:37:00Z"),
            Name = "name-value",
            ContentType = "contentType-value",
            Size = 99,
            IsInline = true,
            Id = "id-value"
        }
    }
};

await graphClient.Groups["{group-id}"].Threads["{conversationThread-id}"].Posts["{post-id}"]
    .Reply(post)
    .Request()
    .PostAsync();

```