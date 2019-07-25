---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 07559c71a1afeee4818c5bc9cfe7dc47955d9d26
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725070"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var subscription = new Subscription
{
    ExpirationDateTime = "2016-11-22T18:23:45.9356913Z"
};

await graphClient.Subscriptions["{id}"]
    .Request()
    .UpdateAsync(subscription);

```