---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d76ddca5c71da8e0d3372ffe38cc8807be6ebe3a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62118929"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ExternalMeetingRegistrant meetingRegistrantBase = new ExternalMeetingRegistrant();
meetingRegistrantBase.id = "9d96988d-a66a-46ce-aad7-0b245615b297";

graphClient.me().onlineMeetings("MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ").registration().registrants()
    .buildRequest()
    .post(meetingRegistrantBase);

```