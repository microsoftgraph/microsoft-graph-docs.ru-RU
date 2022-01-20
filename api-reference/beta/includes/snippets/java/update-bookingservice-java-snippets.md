---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8b7e1bb61b7c62ce5191c269258ba3361d410062
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62094512"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BookingService bookingService = new BookingService();
bookingService.defaultDuration = DatatypeFactory.newInstance().newDuration("PT30M");

graphClient.bookingBusinesses("Contosolunchdelivery@contoso.onmicrosoft.com").services("57da6774-a087-4d69-b0e6-6fb82c339976")
    .buildRequest()
    .patch(bookingService);

```