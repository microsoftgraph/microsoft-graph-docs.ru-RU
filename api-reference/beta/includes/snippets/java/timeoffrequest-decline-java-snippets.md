---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0620813a71ba4ec6a69860bc411da7853683f510
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979288"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String message = "message-value";

graphClient.teams("{teamId}").schedule().timeOffRequests("{timeOffRequestId}")
    .decline(ScheduleChangeRequestDeclineParameterSet
        .newBuilder()
        .withMessage(message)
        .build())
    .buildRequest()
    .post();

```