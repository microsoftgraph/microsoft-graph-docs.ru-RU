---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3458762cfb082f2e40d6222b541476c06c55753b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778531"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var @event = new Event
{
    Location = new Location
    {
        DisplayName = "Conf Room 2"
    }
};

await graphClient.Groups["{group-id}"].Calendar.Events["{event-id}"]
    .Request()
    .UpdateAsync(@event);

```