---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 12f4ea6db913b0635ea4bb0457db95e8b48f302d
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475129"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var temporaryAccessPassAuthenticationMethod = new TemporaryAccessPassAuthenticationMethod
{
    StartDateTime = DateTimeOffset.Parse("2021-01-26T00:00:00Z"),
    LifetimeInMinutes = 60,
    IsUsableOnce = false
};

await graphClient.Users["kim@contoso.com"].Authentication.TemporaryAccessPassMethods
    .Request()
    .AddAsync(temporaryAccessPassAuthenticationMethod);

```