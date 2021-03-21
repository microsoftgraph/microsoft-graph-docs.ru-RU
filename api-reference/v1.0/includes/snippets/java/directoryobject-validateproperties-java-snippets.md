---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: eb73fdea996520598f8f2e8e4f156a468fe47d28
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976852"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String entityType = "Group";

String displayName = "Myprefix_test_mysuffix";

String mailNickname = "Myprefix_test_mysuffix";

UUID onBehalfOfUserId = UUID.fromString("onBehalfOfUserId-value");

graphClient.directoryObjects()
    .validateProperties(DirectoryObjectValidatePropertiesParameterSet
        .newBuilder()
        .withEntityType(entityType)
        .withDisplayName(displayName)
        .withMailNickname(mailNickname)
        .withOnBehalfOfUserId(onBehalfOfUserId)
        .build())
    .buildRequest()
    .post();

```