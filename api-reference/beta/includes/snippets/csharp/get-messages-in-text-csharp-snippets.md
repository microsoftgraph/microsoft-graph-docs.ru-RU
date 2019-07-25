---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 849d211946832342d49558189d4834ecf35bb6c1
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724091"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messages = await graphClient.Me.Messages
    .Request()
    .Header("Prefer","outlook.body-content-type=\"text\"")
    .Select( e => new {
             e.Subject,
             e.Body,
             e.BodyPreview,
             e.UniqueBody 
             })
    .GetAsync();

```