---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 34bed3bfb59a531b155e88722aa2eb67cafbfb0b9b0887fc828dd21b73cffd53
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57052387"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LanguageProficiency languageProficiency = new LanguageProficiency();
languageProficiency.allowedAudiences = EnumSet.of(AllowedAudiences.ORGANIZATION);

graphClient.me().profile().languages("{id}")
    .buildRequest()
    .patch(languageProficiency);

```