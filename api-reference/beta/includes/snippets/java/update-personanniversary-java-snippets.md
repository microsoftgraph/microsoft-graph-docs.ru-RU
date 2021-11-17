---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 18cbac6905edacc9114a2f6074fbcc0bbc8af2b382036985c5f592579563732c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57196229"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonAnnualEvent personAnnualEvent = new PersonAnnualEvent();
personAnnualEvent.allowedAudiences = EnumSet.of(AllowedAudiences.CONTACTS);

graphClient.me().profile().anniversaries("{id}")
    .buildRequest()
    .patch(personAnnualEvent);

```