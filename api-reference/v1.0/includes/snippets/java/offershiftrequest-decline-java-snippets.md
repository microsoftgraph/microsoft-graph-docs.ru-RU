---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7e5077024f3bf9d1acd328d09a28dd5fcc48a4f58f2072357f187b0496dd6985
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57366790"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String message = "Sorry, you can't offer this shift.";

graphClient.teams("{teamId}").schedule().offerShiftRequests("{offerShiftRequestId}")
    .decline(ScheduleChangeRequestDeclineParameterSet
        .newBuilder()
        .withMessage(message)
        .build())
    .buildRequest()
    .post();

```