---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0113ff8703a0674135eb8340bb395872a3aa6395
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2021
ms.locfileid: "51211138"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> userIdsList = new LinkedList<String>();
userIdsList.add("29f270bb-4d23-4f68-8a57-dc73dc0d4caf");

graphClient.identityProtection().riskyUsers()
    .confirmCompromised(RiskyUserConfirmCompromisedParameterSet
        .newBuilder()
        .withUserIds(userIdsList)
        .build())
    .buildRequest()
    .post();

```