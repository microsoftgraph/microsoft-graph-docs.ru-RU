---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e6b3a5136c45295bf916df1614c71d8c85ef181f
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65205541"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BookingBusinessGetStaffAvailabilityCollectionPage getStaffAvailability = graphClient.bookingBusinesses("Contosolunchdelivery@contoso.onmicrosoft.com")
    .getStaffAvailability()
    .buildRequest()
    .get();

```