---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e182135c8341fc34be221b35f1cddd4384e4076b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802038"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingCustomer = await graphClient.BookingBusinesses["{bookingBusiness-id}"].Customers["{bookingCustomer-id}"]
    .Request()
    .GetAsync();

```