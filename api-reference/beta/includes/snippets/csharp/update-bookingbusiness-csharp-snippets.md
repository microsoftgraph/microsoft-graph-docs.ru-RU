---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 48ecb124281169a4eeb6424272baa6a76e4e69cb
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35506070"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingBusiness = new BookingBusiness
{
    Email = "admin@fabrikam.com",
    SchedulingPolicy = new BookingSchedulingPolicy
    {
        TimeSlotInterval = "PT60M",
        MinimumLeadTime = "P1D",
        MaximumAdvance = "P30D",
        SendConfirmationsToOwner = true,
        AllowStaffSelection = true
    }
};

await graphClient.BookingBusinesses["fabrikam@M365B489948.onmicrosoft.com"]
    .Request()
    .UpdateAsync(bookingBusiness);

```