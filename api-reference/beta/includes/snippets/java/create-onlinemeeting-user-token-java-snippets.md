---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 77120bfb33fac75d8a487d23f0cd201d2d8680d4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978975"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OnlineMeeting onlineMeeting = new OnlineMeeting();
onlineMeeting.startDateTime = OffsetDateTimeSerializer.deserialize("2019-07-12T21:30:34.2444915+00:00");
onlineMeeting.endDateTime = OffsetDateTimeSerializer.deserialize("2019-07-12T22:00:34.2464912+00:00");
onlineMeeting.subject = "User Token Meeting";

graphClient.me().onlineMeetings()
    .buildRequest()
    .post(onlineMeeting);

```