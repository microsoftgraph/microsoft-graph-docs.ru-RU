---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ee77fde725e33beaba53fec3848f6d992b254864
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62130011"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BookingBusiness bookingBusiness = new BookingBusiness();
bookingBusiness.email = "admin@fabrikam.com";
BookingSchedulingPolicy schedulingPolicy = new BookingSchedulingPolicy();
schedulingPolicy.timeSlotInterval = DatatypeFactory.newInstance().newDuration("PT60M");
schedulingPolicy.minimumLeadTime = DatatypeFactory.newInstance().newDuration("P1D");
schedulingPolicy.maximumAdvance = DatatypeFactory.newInstance().newDuration("P30D");
schedulingPolicy.sendConfirmationsToOwner = true;
schedulingPolicy.allowStaffSelection = true;
bookingBusiness.schedulingPolicy = schedulingPolicy;

graphClient.bookingBusinesses("fabrikam@contoso.onmicrosoft.com")
    .buildRequest()
    .patch(bookingBusiness);

```