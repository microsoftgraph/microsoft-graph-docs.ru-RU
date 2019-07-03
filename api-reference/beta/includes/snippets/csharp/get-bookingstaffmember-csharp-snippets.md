---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f25e4abdc267e2625481c248a9372aed2b436f2c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35505360"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingStaffMember = await graphClient.BookingBusinesses["Contosolunchdelivery@M365B489948.onmicrosoft.com"].StaffMembers["71d64d0e-7225-49b6-b0b1-070d476cda51"]
    .Request()
    .GetAsync();

```