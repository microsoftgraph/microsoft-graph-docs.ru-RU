---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4b02e01caba33282f07b4462d14022d2155c5e7b9e538cf716a253953dfaa58f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57139735"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> userIdsList = new LinkedList<String>();
userIdsList.add("29f270bb-4d23-4f68-8a57-dc73dc0d4caf");
userIdsList.add("20f91ec9-d140-4d90-9cd9-f618587a1471");

graphClient.riskyUsers()
    .confirmCompromised(RiskyUserConfirmCompromisedParameterSet
        .newBuilder()
        .withUserIds(userIdsList)
        .build())
    .buildRequest()
    .post();

```