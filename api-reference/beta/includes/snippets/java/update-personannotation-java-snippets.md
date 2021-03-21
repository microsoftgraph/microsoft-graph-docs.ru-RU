---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d2aaa85b57622c327fe02074f72b8e2d4c679d79
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971164"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonAnnotation personAnnotation = new PersonAnnotation();
personAnnotation.allowedAudiences = EnumSet.of(AllowedAudiences.ORGANIZATION);

graphClient.users("{userId}").profile().notes("{id}")
    .buildRequest()
    .patch(personAnnotation);

```