---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d8721e3bc2c151ee301a9436d9d95e1238b5b4d2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50970204"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DateTimeTimeZone newReminderTime = new DateTimeTimeZone();
newReminderTime.dateTime = "dateTime-value";
newReminderTime.timeZone = "timeZone-value";

graphClient.me().events("{id}")
    .snoozeReminder(EventSnoozeReminderParameterSet
        .newBuilder()
        .withNewReminderTime(newReminderTime)
        .build())
    .buildRequest()
    .post();

```