---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 66a4b57838731577c417f26051279f78c0e948fe
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62109766"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BookingAppointmentCollectionPage appointments = graphClient.bookingBusinesses("Contosolunchdelivery@contoso.onmicrosoft.com").appointments()
    .buildRequest()
    .get();

```