---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: cdd28f321b7cfa7c1881652e967c11d28a2c12391475e5fe6edf4e4d34cfd01e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57260928"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonAnnotation personAnnotation = new PersonAnnotation();
personAnnotation.allowedAudiences = EnumSet.of(AllowedAudiences.ORGANIZATION);

graphClient.users("{userId}").profile().notes("{id}")
    .buildRequest()
    .patch(personAnnotation);

```