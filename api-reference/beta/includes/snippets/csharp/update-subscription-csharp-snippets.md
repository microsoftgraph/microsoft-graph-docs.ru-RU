---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e76cfeba545c12c7cc18598eba44c58a26672ff0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800609"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var subscription = new Subscription
{
    ExpirationDateTime = DateTimeOffset.Parse("2016-11-22T18:23:45.9356913Z")
};

await graphClient.Subscriptions["{subscription-id}"]
    .Request()
    .UpdateAsync(subscription);

```