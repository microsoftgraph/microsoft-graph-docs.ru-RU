---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4a15922bb9692ab7b0593c283022d7fd76ecaf2c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960875"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> userIdsList = new LinkedList<String>();
userIdsList.add("04487ee0-f4f6-4e7f-8999-facc5a30e232");

graphClient.identityProtection().riskyUsers()
    .dismiss(userIdsList)
    .buildRequest()
    .post();

```