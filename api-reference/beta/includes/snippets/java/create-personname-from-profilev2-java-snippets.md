---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d04b262a678782c65aad0362cccd002cf492a8be
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981741"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonName personName = new PersonName();
personName.displayName = "Innocenty Popov";
personName.first = "Innocenty";
personName.initials = "IP";
personName.last = "Popov";
personName.languageTag = "en-US";
personName.maiden = null;

graphClient.me().profile().names()
    .buildRequest()
    .post(personName);

```