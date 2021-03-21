---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 287d3a9df442116f1ed3df5c0f05628cc13ed111
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971020"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LanguageProficiency languageProficiency = new LanguageProficiency();
languageProficiency.allowedAudiences = EnumSet.of(AllowedAudiences.ORGANIZATION);

graphClient.me().profile().languages("{id}")
    .buildRequest()
    .patch(languageProficiency);

```