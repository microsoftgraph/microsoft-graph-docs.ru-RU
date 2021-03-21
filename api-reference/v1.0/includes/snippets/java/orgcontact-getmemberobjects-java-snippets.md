---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: dbd9f956ab3b6036f9962d39a0a632c86f28502c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977441"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Boolean securityEnabledOnly = false;

graphClient.contacts("{id}")
    .getMemberObjects(DirectoryObjectGetMemberObjectsParameterSet
        .newBuilder()
        .withSecurityEnabledOnly(securityEnabledOnly)
        .build())
    .buildRequest()
    .post();

```