---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7c068b9c67ea850d3c6d2166d92707542ab31123
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2020
ms.locfileid: "44683632"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = new ReferenceAttachment
{
    Name = "Personal pictures",
    SourceUrl = "https://contoso.com/personal/mario_contoso_net/Documents/Pics",
    ProviderType = ReferenceAttachmentProvider.OneDriveConsumer,
    Permission = ReferenceAttachmentPermission.Edit,
    IsFolder = true
};

await graphClient.Me.Messages["AAMkAGE1M88AADUv0uFAAA="].Attachments
    .Request()
    .AddAsync(attachment);

```