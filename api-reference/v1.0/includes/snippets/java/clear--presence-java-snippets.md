---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8b453148281c1d7e7b29f4d0963aac5abf2aa5d3
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/25/2021
ms.locfileid: "58514232"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String sessionId = "22553876-f5ab-4529-bffb-cfe50aa89f87";

graphClient.users("fa8bf3dc-eca7-46b7-bad1-db199b62afc3").presence()
    .clearPresence(PresenceClearPresenceParameterSet
        .newBuilder()
        .withSessionId(sessionId)
        .build())
    .buildRequest()
    .post();

```