---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 601383a5837e077b8f5c69fabae327e8b8329218
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/24/2021
ms.locfileid: "53578829"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Applications["{application-id}"]
    .UnsetVerifiedPublisher()
    .Request()
    .PostAsync();

```