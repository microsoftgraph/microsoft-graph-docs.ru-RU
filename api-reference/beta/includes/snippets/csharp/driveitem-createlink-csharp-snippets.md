---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 06dd247bc9cc00d1a41be44095364dccbb979138
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "52990740"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var type = "view";

var scope = "anonymous";

var password = "String";

var recipients = new List<DriveRecipient>()
{
    new DriveRecipient
    {
    }
};

await graphClient.Me.Drive.Items["{driveItem-id}"]
    .CreateLink(type,scope,null,password,null,recipients)
    .Request()
    .PostAsync();

```