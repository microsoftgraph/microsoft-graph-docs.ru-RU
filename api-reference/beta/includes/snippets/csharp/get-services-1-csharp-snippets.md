---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a09ca76469ea074c84710441d6a553867f8e2959f2e5cbae6d3713eca5d8ca7d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57199279"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var services = await graphClient.BookingBusinesses["{bookingBusiness-id}"].Services
    .Request()
    .GetAsync();

```