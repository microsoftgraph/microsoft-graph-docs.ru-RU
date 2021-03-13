---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: cd5b8a64bff6058f8f2192c362dd65f87c642808
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788694"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingBusiness = await graphClient.BookingBusinesses["{bookingBusiness-id}"]
    .Request()
    .GetAsync();

```